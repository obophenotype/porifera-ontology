# This Makefile is for use by the PORO Release Manager.
#
# requirements: Oort (http://code.google.com/p/owltools/wiki/OortIntro)
#
# To make a release, type 'make release' in this directory

build: poro.obo minidiff
release: poro.obo diff

# all release files are derived from the editors version.
# we use the default Oort setup (hermit as reasoner)
poro.obo: poro-edit.ofn
	ontology-release-runner $< --allow-overwrite --asserted --simple

obo2owl:
	obolib-owl2obo poro-edit.owl -o poro-edit.obo

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
# Diffs
# ----------------------------------------

# 
diff: poro.obo
	cd diffs && touch poro-diff && rm poro-*diff* && make

# Minidiff: intra-release differences
# TESTING: emailing self, will change to list
minidiff: poro.obo
	cd diffs  && touch poro-diff && rm poro-*diff* && make TGTS='html txt' SRC=../poro.obo && mail -s poro-diffs cjmungall@lbl.gov < poro-combined-diff.txt
