OBO=http://purl.obolibrary.org/obo
ONT = poro
SRC = ../$(ONT).obo
LAST = $(OBO)/$(ONT).obo
OWLSRC = ../$(ONT).owl
OWLLAST = $(OBO)/$(ONT).owl

all: $(ONT)-obo-diff.html $(ONT)-def-diff.html $(ONT)-lastbuild.obo $(ONT)-combined-diff.txt 
qll_release: all $(ONT)-diff.md

$(ONT)-obo-diff.html: $(ONT)-lastbuild.obo $(SRC)
	compare-obo-files.pl --config 'html/ontology_name=$(ONT)' --rss-path . -f1 $< -f2 $(SRC) -m html text rss -o $(ONT)-obo-diff && replace-amigo-urls-with-purls.pl $@
$(ONT)-def-diff.html: $(ONT)-lastbuild.obo $(SRC)
	compare-defs.pl --config 'html/ontology_name=$(ONT)' --rss-path . -f1 $< -f2 $(SRC) -m html text rss -o $(ONT)-def-diff && replace-amigo-urls-with-purls.pl $@

$(ONT)-combined-diff.txt: $(ONT)-def-diff.html $(ONT)-obo-diff.html
	cat $(ONT)-def-diff.txt $(ONT)-obo-diff.txt > $@

$(ONT)-lastbuild.obo: $(SRC)
	wget --no-check-certificate $(LAST) -O $@

$(ONT)-lastbuild.owl: $(SRC)
	wget --no-check-certificate $(OWLLAST) -O $@ && touch $@

$(ONT)-diff.md: $(ONT)-lastbuild.owl $(OWLSRC)
	owljs-diff -C ../catalog-v001.xml -o $@ $< $(OWLSRC) 

