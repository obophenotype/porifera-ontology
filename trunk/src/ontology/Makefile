poro.obo: poro-edit.ofn
	ontology-release-runner $< --allow-overwrite --asserted --simple

obo2owl:
	obolib-owl2obo poro-edit.owl -o poro-edit.obo

poro-parse.obo: all.html
	./parse.pl $< > $@

porifera-taxonomy.obo:
	blip ontol-query -r taxonomy -query "class(X,'Porifera'),(subclassRT(X,ID);subclassT(ID,X))" -to obo > $@

porifera-taxonomy.owl: porifera.obo
	owltools $< -o -f functional file://`pwd`/$@

poro-edit.rdf: poro-edit.owl
	owltools $< -o file://`pwd`/$@

np.txt: poro.obo
	blip-findall -i $< "class(X),\+subclass(X,Y)" -select X -label > $@ && wc $@
