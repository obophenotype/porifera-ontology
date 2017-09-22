OBO=http://purl.obolibrary.org/obo
ONT=poro
BASE=$(OBO)/$(ONT)
SRC=$(ONT)-edit.owl
RELEASEDIR=../..
ROBOT= robot
OWLTOOLS= owltools
USECAT= --use-catalog

all: all_imports $(ONT).owl $(ONT).obo
products: $(ONT).owl $(ONT).obo
test: products
phenote-test: test oetest

oetest: poro.obo
	obo2obo $< -o /dev/null

release: $(ONT).owl $(ONT).obo
	cp $^ $(RELEASEDIR) && cp imports/* $(RELEASEDIR)/imports

prepare_release: all
	cp $(ONT).owl $(ONT).obo $(RELEASEDIR) &&\
	mkdir -p $(RELEASEDIR)/imports &&\
	cp imports/*{owl,obo} $(RELEASEDIR)/imports &&\
	git add $(RELEASEDIR)/imports/*{obo,owl} &&\
	(test -f subsets/*owl && cp subsets/*{owl,obo} $(RELEASEDIR)/subsets && git add $(RELEASEDIR)/subsets/* || echo "no subsets") &&\
	echo "Release files are now in $(RELEASEDIR) - now you should commit, push and make a release on github"

$(ONT).owl: $(SRC)
	$(ROBOT)  reason -i $< -r ELK relax reduce -r ELK annotate -V $(BASE)/releases/`date +%Y-%m-%d`/$(ONT).owl -o $@
$(ONT).obo: $(ONT).owl
	$(OWLTOOLS) $(USECAT)  $< --merge-imports-closure --add-obo-shorthand-to-properties -o -f obo --no-check $(ONT).tmp.obo && grep -v ^owl-axioms $(ONT).tmp.obo > $@

$(ONT)-edit.ttl: $(ONT)-edit.owl
	$(ROBOT) convert -i $< -o $@

IMPORTS = pato uberon chebi cl go
IMPORTS_OWL = $(patsubst %, imports/%_import.owl,$(IMPORTS)) $(patsubst %, imports/%_import.obo,$(IMPORTS))

# Make this target to regenerate ALL
all_imports: $(IMPORTS_OWL)

imports/seed.txt: poro-edit.ttl
	arq --data $< --query sparql/getSeed.rq --out TSV > $@.tmp && sort -u $@.tmp | perl -npe 's@^<@@;s@>$$@@' > $@
#	$(OWLTOOLS) $(USECAT) $< --export-table $@.tmp && cut -f1 $@.tmp > $@

# Use ROBOT, driven entirely by terms lists NOT from source ontology
imports/%_import.owl: mirror/%.owl imports/seed.txt
	ROBOT_JAVA_ARGS="-Xmx4G" $(ROBOT) extract -i $< -T imports/seed.txt --method BOT -O $(BASE)/$@ -o $@
.PRECIOUS: imports/%_import.owl

imports/%_import.obo: imports/%_import.owl
	$(OWLTOOLS) $(USECAT) $< -o -f obo $@

# clone remote ontology locally, perfoming some excision of relations and annotations
mirror/%.obo: $(SRC)
	mkdir -p mirror &&\
	wget --no-check-certificate $(OBO)/$*.obo -O $@ && touch $@
.PRECIOUS: mirror/%.obo

mirror/%.owl: mirror/%.obo
	$(OWLTOOLS) $< --merge-imports-closure --remove-axiom-annotations --remove-annotation-assertions -l -s -d -r --remove-dangling-annotations  -o $@
.PRECIOUS: mirror/%.owl

mirror/ro.owl: $(SRC)
	$(OWLTOOLS) $(OBO)/ro.owl --merge-imports-closure --remove-annotation-assertions -l -s -d -r --remove-dangling-annotations  -o $@
.PRECIOUS: mirror/%.owl


