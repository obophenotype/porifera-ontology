# This Makefile is for use by the PORO Release Manager.
#
# requirements: Oort (http://code.google.com/p/owltools/wiki/OortIntro)
#
# To make a release, type 'make release' in this directory

OBO = http://purl.obolibrary.org/obo/
RELEASE = $(OBO)/ceph/releases/`date +%Y-%m-%d`

build: poro.obo poro.owl minidiff
release: poro.obo diff copy-release

TARGETS = poro.obo poro.owl imports diffs
copy-release:
	cp -pr $(TARGETS) ../.. && cd ../.. && git add imports/*

USECAT= --use-catalog

# all release files are derived from the editors version.
# we use the default Oort setup (hermit as reasoner)
build/poro.owl: poro-edit.owl
	ontology-release-runner --catalog-xml catalog-v001.xml $< --allow-overwrite --asserted --simple --outdir build

build/%: build/poro.owl
poro.owl: build/poro.owl
	cp $< $@
.PRECIOUS: poro.owl
poro.obo: poro.owl
	owltools $(USECAT) $< --merge-imports-closure -o -f obo --no-check $@

poro-parse.obo: all.html
	./parse.pl $< > $@

porifera-taxonomy.obo:
	blip ontol-query -r taxonomy -query "class(X,'Porifera'),(subclassRT(X,ID);subclassT(ID,X))" -to obo > $@

porifera-taxonomy.owl: porifera-taxonomy.obo
	owltools $< -o file://`pwd`/$@

poro-edit.rdf: poro-edit.owl
	owltools $< -o file://`pwd`/$@

np.txt: poro.obo
	blip-findall -i $< "class(X),\+subclass(X,Y)" -select X -label > $@ && wc $@

poro-parts.owl: poro-edit.ofn
	owltools --use-catalog --create-ontology poro-parts $< --materialize-existentials -p BFO:0000050 --add-imports-from-supports -o $@

# ----------------------------------------
# Bridges
# ----------------------------------------
core.owl: poro.owl
	owltools --use-catalog $< --extract-bridge-ontologies -x -d . -s poro --remove-imports-declarations -o core.owl

# ----------------------------------------
# Regenerate imports
# ----------------------------------------
# Uses OWLAPI Module Extraction code

# Type 'make imports/X_import.owl' whenever you wish to refresh the import for an ontology X. This is when:
#
#  1. X has changed and we want to include these changes
#  2. We have added onr or more new IRI from X into poro-edit.owl
#  3. We have removed references to one or more IRIs in X from poro-edit.owl
#
# You should NOT edit these files directly, changes will be overwritten.
#
# If you want to add something to these, edit poro-edit.owl and add an axiom with a IRI from X. You don't need to add any information about X.

# Base URI for local subset imports
PORO_IMPORTS_BASE_URI = $(OBO)/poro/imports

# Ontology dependencies
IMPORTS = pato uberon chebi cl go

# Make this target to regenerate ALL
all_imports: $(patsubst %, imports/%_import.owl,$(IMPORTS)) $(patsubst %, imports/%_import.obo,$(IMPORTS))

KEEPRELS = BFO:0000050 BFO:0000051 RO:0002202 immediate_transformation_of

# Create an import module using the OWLAPI module extraction code via OWLTools.
# We use the standard catalog, but rewrite the import to X to be a local mirror of ALL of X.
# After extraction, we further reduce the ontology by creating a "mingraph" (removes all annotations except label) and by 
imports/%_import.owl: poro-edit.owl mirror/%.owl
	owltools  $(USECAT) --map-ontology-iri $(PORO_IMPORTS_BASE_URI)/$*_import.owl mirror/$*.owl  $<  --extract-module -s $(OBO)/$*.owl -c --remove-axiom-annotations --make-subset-by-properties -f $(KEEPRELS)  --set-ontology-id $(OBO)/poro/$@ -o file://`pwd`/$@


imports/ro_import.owl: poro-edit.owl mirror/ro.owl
	owltools  $(USECAT) --map-ontology-iri $(PORO_IMPORTS_BASE_URI)/ro_import.owl mirror/ro.owl  $<  --extract-module -s $(OBO)/ro.owl -c --remove-axiom-annotations --set-ontology-id $(OBO)/poro/$@ -o file://`pwd`/$@

# clone remote ontology locally, perfoming some excision of relations and annotations
mirror/%.owl:
	owltools $(OBO)/$*.owl --remove-annotation-assertions -l --remove-dangling-annotations  --make-subset-by-properties -f $(KEEPRELS)  --set-ontology-id $(OBO)/$*.owl -o $@
mirror/ro.owl:
	wget $(OBO)/ro.owl -O $@
mirror/uberon.owl:
	owltools $(OBO)/uberon/basic.owl --remove-annotation-assertions -l -s -d --remove-axiom-annotations --remove-dangling-annotations --make-subset-by-properties -f $(KEEPRELS) --set-ontology-id $(OBO)/uberon.owl -o $@
mirror/pr.obo:
	wget $(OBO)/pr.obo -O $@.tmp && obo-grep.pl -r 'id: PR:' $@.tmp > $@
mirror/pr.owl: mirror/pr.obo
	owltools $< --remove-dangling --set-ontology-id $(OBO)/pr.owl -o $@
.PRECIOUS: mirror/%.owl

imports/%_import.obo: imports/%_import.owl
	owltools $< -o -f obo $@

# ----------------------------------------
# Diffs
# ----------------------------------------

# 
diff: poro.obo
	cd diffs && touch poro-diff && rm poro-*diff* && make all_release

# Minidiff: intra-release differences
# TESTING: emailing self, will change to list
minidiff: poro.obo
	cd diffs  && touch poro-diff && rm poro-*diff* && make TGTS='html txt' SRC=../poro.obo && mail -s poro-diffs cjmungall@lbl.gov < poro-combined-diff.txt
