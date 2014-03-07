---
title: "/releases/2014-01-03/poro.owl"
date: "2014-01-03"
summary: ""
categories: release
image: '/anatomy/images/u-logo.jpg
tags:
 - release
---

# Ontology Diff Report


## Original Ontology

 * IRI: http://purl.obolibrary.org/obo/poro.owl
 * VersionIRI: http://purl.obolibrary.org/obo/poro/releases/2014-01-03/poro.owl

## New Ontology

 * IRI: http://purl.obolibrary.org/obo/poro.owl
 * VersionIRI: http://purl.obolibrary.org/obo/poro/releases/2014-01-03/poro.owl

# Report for classes


## Class objects lost from source: 0


## Class objects new in target: 1


### New Class : [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004)

 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000111* independent continuant
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* a heart
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *[label](http://www.w3.org/2000/01/rdf-schema#label)* independent continuant
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) **SubClassOf** [continuant](http://purl.obolibrary.org/obo/BFO_0000002)
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000118* substantial entity
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* an organism
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* A continuant that is a bearer of quality and realizable entity entities, in which other entities inhere and which itself cannot inhere in anything.
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* a chair
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* a symphony orchestra
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* the bottom right portion of a human torso
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* a person
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* a leg
 * [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) *http://purl.obolibrary.org/obo/IAO_0000112* the lawn and atmosphere in front of our building

## Changed Class objects: 43


### Changes for: [reproduction](http://purl.obolibrary.org/obo/GO_0000003)

 * _Added_
    *  **+** [reproduction](http://purl.obolibrary.org/obo/GO_0000003) **SubClassOf** [biological process](http://purl.obolibrary.org/obo/GO_0008150)

### Changes for: [multispicular fiber](http://purl.obolibrary.org/obo/PORO_0000414)

 * _Deleted_
    *  **-** [multispicular fiber](http://purl.obolibrary.org/obo/PORO_0000414) **SubClassOf** ObjectMinCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule](http://purl.obolibrary.org/obo/PORO_0000017) ) 
 * _Added_
    *  **+** [multispicular fiber](http://purl.obolibrary.org/obo/PORO_0000414) **SubClassOf** ObjectMinCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule](http://purl.obolibrary.org/obo/PORO_0000017) ) 

### Changes for: [monaene](http://purl.obolibrary.org/obo/PORO_0000411)

 * _Deleted_
    *  **-** [monaene](http://purl.obolibrary.org/obo/PORO_0000411) **EquivalentTo** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
    *  **-** [monaene](http://purl.obolibrary.org/obo/PORO_0000411) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
 * _Added_
    *  **+** [monaene](http://purl.obolibrary.org/obo/PORO_0000411) **EquivalentTo** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
    *  **+** [monaene](http://purl.obolibrary.org/obo/PORO_0000411) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 

### Changes for: [micropyle](http://purl.obolibrary.org/obo/PORO_0000406)

 * _Added_
    *  **+** [micropyle](http://purl.obolibrary.org/obo/PORO_0000406) **SubClassOf** [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004)

### Changes for: [gemmule coat](http://purl.obolibrary.org/obo/PORO_0000928)

 * _Deleted_
    *  **-** [gemmule coat](http://purl.obolibrary.org/obo/PORO_0000928) **SubClassOf** [surrounds](http://purl.obolibrary.org/obo/sponge#surrounds) **some** [gemmule](http://purl.obolibrary.org/obo/PORO_0000330)
 * _Added_
    *  **+** [gemmule coat](http://purl.obolibrary.org/obo/PORO_0000928) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002221 **some** [gemmule](http://purl.obolibrary.org/obo/PORO_0000330)

### Changes for: [aragonite](http://purl.obolibrary.org/obo/CHEBI_52239)

 * _Deleted_
    *  **-** [aragonite](http://purl.obolibrary.org/obo/CHEBI_52239) **SubClassOf** [chemical entity](http://purl.obolibrary.org/obo/CHEBI_24431)
 * _Added_
    *  **+** [aragonite](http://purl.obolibrary.org/obo/CHEBI_52239) **SubClassOf** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311)
    *  **+** [aragonite](http://purl.obolibrary.org/obo/CHEBI_52239) **SubClassOf** [carbonate mineral](http://purl.obolibrary.org/obo/CHEBI_46720)
    *  **+** [aragonite](http://purl.obolibrary.org/obo/CHEBI_52239) *[label](http://www.w3.org/2000/01/rdf-schema#label)* aragonite

### Changes for: [larva](http://purl.obolibrary.org/obo/UBERON_0002548)

 * _Added_
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) **SubClassOf** [multi-cellular organism](http://purl.obolibrary.org/obo/UBERON_0000468)
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* a distinct juvenile form many animals undergo before metamorphosis into adults. Animals with indirect development such as insects, amphibians, or cnidarians typically have a larval phase of their life cycle.
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has exact synonym](http://www.geneontology.org/formats/oboInOwl#hasExactSynonym)* larval organism
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* ammocoete
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* bipinnaria
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* caterpillar
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* glochidium
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* grub
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* leptocephalus
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* maggot
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* naiad
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* nymph
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* planula
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* tadpole
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* trochophore
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* veliger
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* wriggler
    *  **+** [larva](http://purl.obolibrary.org/obo/UBERON_0002548) *[has narrow synonym](http://www.geneontology.org/formats/oboInOwl#hasNarrowSynonym)* zoea

### Changes for: [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311)

 * _Deleted_
    *  **-** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311) **SubClassOf** [chemical entity](http://purl.obolibrary.org/obo/CHEBI_24431)
 * _Added_
    *  **+** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311) **SubClassOf** [calcium salt](http://purl.obolibrary.org/obo/CHEBI_35156)
    *  **+** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311) **SubClassOf** [carbonate salt](http://purl.obolibrary.org/obo/CHEBI_46721)
    *  **+** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311) **SubClassOf** [one-carbon compound](http://purl.obolibrary.org/obo/CHEBI_64708)
    *  **+** [calcium carbonate](http://purl.obolibrary.org/obo/CHEBI_3311) *[label](http://www.w3.org/2000/01/rdf-schema#label)* calcium carbonate

### Changes for: [triaxone](http://purl.obolibrary.org/obo/PORO_0000602)

 * _Deleted_
    *  **-** [triaxone](http://purl.obolibrary.org/obo/PORO_0000602) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [ray axis](http://purl.obolibrary.org/obo/PORO_0000909) ) 
    *  **-** [triaxone](http://purl.obolibrary.org/obo/PORO_0000602) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [ray axis](http://purl.obolibrary.org/obo/PORO_0000909) ) 
 * _Added_
    *  **+** [triaxone](http://purl.obolibrary.org/obo/PORO_0000602) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [ray axis](http://purl.obolibrary.org/obo/PORO_0000909) ) 
    *  **+** [triaxone](http://purl.obolibrary.org/obo/PORO_0000602) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [ray axis](http://purl.obolibrary.org/obo/PORO_0000909) ) 

### Changes for: [triactine](http://purl.obolibrary.org/obo/PORO_0000600)

 * _Deleted_
    *  **-** [triactine](http://purl.obolibrary.org/obo/PORO_0000600) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
    *  **-** [triactine](http://purl.obolibrary.org/obo/PORO_0000600) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
 * _Added_
    *  **+** [triactine](http://purl.obolibrary.org/obo/PORO_0000600) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
    *  **+** [triactine](http://purl.obolibrary.org/obo/PORO_0000600) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 

### Changes for: [triaene](http://purl.obolibrary.org/obo/PORO_0000601)

 * _Deleted_
    *  **-** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
    *  **-** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [rhabd](http://purl.obolibrary.org/obo/PORO_0000500) ) 
    *  **-** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
    *  **+** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [rhabd](http://purl.obolibrary.org/obo/PORO_0000500) ) 
    *  **+** [triaene](http://purl.obolibrary.org/obo/PORO_0000601) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [phagocytosis](http://purl.obolibrary.org/obo/GO_0006909)

 * _Deleted_
    *  **-** [phagocytosis](http://purl.obolibrary.org/obo/GO_0006909) **SubClassOf** [biological process](http://purl.obolibrary.org/obo/GO_0008150)
 * _Added_
    *  **+** [phagocytosis](http://purl.obolibrary.org/obo/GO_0006909) **SubClassOf** [endocytosis](http://purl.obolibrary.org/obo/GO_0006897)
    *  **+** [phagocytosis](http://purl.obolibrary.org/obo/GO_0006909) **SubClassOf** [single-organism transport](http://purl.obolibrary.org/obo/GO_0044765)

### Changes for: [anatomical structure](http://purl.obolibrary.org/obo/CARO_0000003)

 * _Added_
    *  **+** [anatomical structure](http://purl.obolibrary.org/obo/CARO_0000003) *[label](http://www.w3.org/2000/01/rdf-schema#label)* anatomical structure
    *  **+** [anatomical structure](http://purl.obolibrary.org/obo/CARO_0000003) *http://purl.obolibrary.org/obo/IAO_0000412* http://purl.obolibrary.org/obo/caro.owl

### Changes for: [material anatomical entity](http://purl.obolibrary.org/obo/CARO_0000006)

 * _Added_
    *  **+** [material anatomical entity](http://purl.obolibrary.org/obo/CARO_0000006) **SubClassOf** [material entity](http://purl.obolibrary.org/obo/BFO_0000040)
    *  **+** [material anatomical entity](http://purl.obolibrary.org/obo/CARO_0000006) *[label](http://www.w3.org/2000/01/rdf-schema#label)* material anatomical entity
    *  **+** [material anatomical entity](http://purl.obolibrary.org/obo/CARO_0000006) *http://purl.obolibrary.org/obo/IAO_0000412* http://purl.obolibrary.org/obo/caro.owl

### Changes for: [germ line cell](http://purl.obolibrary.org/obo/CL_0000039)

 * _Added_
    *  **+** [germ line cell](http://purl.obolibrary.org/obo/CL_0000039) **SubClassOf** [animal cell](http://purl.obolibrary.org/obo/CL_0000548)

### Changes for: [chemical entity](http://purl.obolibrary.org/obo/CHEBI_24431)

 * _Added_
    *  **+** [chemical entity](http://purl.obolibrary.org/obo/CHEBI_24431) *[label](http://www.w3.org/2000/01/rdf-schema#label)* chemical entity

### Changes for: [cavity of canal](http://purl.obolibrary.org/obo/PORO_0000991)

 * _Deleted_
    *  **-** [cavity of canal](http://purl.obolibrary.org/obo/PORO_0000991) **SubClassOf** [surrounded by](http://purl.obolibrary.org/obo/PORO_0000939) **some** [canal](http://purl.obolibrary.org/obo/PORO_0000039)
 * _Added_
    *  **+** [cavity of canal](http://purl.obolibrary.org/obo/PORO_0000991) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002219 **some** [canal](http://purl.obolibrary.org/obo/PORO_0000039)

### Changes for: [spermatocyte](http://purl.obolibrary.org/obo/CL_0000017)

 * _Deleted_
    *  **-** [spermatocyte](http://purl.obolibrary.org/obo/CL_0000017) **SubClassOf** [germ line cell](http://purl.obolibrary.org/obo/CL_0000039)
 * _Added_
    *  **+** [spermatocyte](http://purl.obolibrary.org/obo/CL_0000017) **SubClassOf** [develops from](http://purl.obolibrary.org/obo/RO_0002202) **some** [spermatogonium](http://purl.obolibrary.org/obo/CL_0000020)
    *  **+** [spermatocyte](http://purl.obolibrary.org/obo/CL_0000017) **SubClassOf** [male germ cell](http://purl.obolibrary.org/obo/CL_0000015)

### Changes for: [calcite](http://purl.obolibrary.org/obo/CHEBI_46719)

 * _Added_
    *  **+** [calcite](http://purl.obolibrary.org/obo/CHEBI_46719) **SubClassOf** [carbonate mineral](http://purl.obolibrary.org/obo/CHEBI_46720)
    *  **+** [calcite](http://purl.obolibrary.org/obo/CHEBI_46719) *[label](http://www.w3.org/2000/01/rdf-schema#label)* calcite

### Changes for: [portion of tissue](http://purl.obolibrary.org/obo/CARO_0000043)

 * _Deleted_
    *  **-** [portion of tissue](http://purl.obolibrary.org/obo/CARO_0000043) **SubClassOf** [surrounds](http://purl.obolibrary.org/obo/sponge#surrounds) **some** [choanochamber](http://purl.obolibrary.org/obo/PORO_0000197)
 * _Added_
    *  **+** [portion of tissue](http://purl.obolibrary.org/obo/CARO_0000043) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002221 **some** [choanochamber](http://purl.obolibrary.org/obo/PORO_0000197)

### Changes for: [oocyte](http://purl.obolibrary.org/obo/CL_0000023)

 * _Deleted_
    *  **-** [oocyte](http://purl.obolibrary.org/obo/CL_0000023) **SubClassOf** [germ line cell](http://purl.obolibrary.org/obo/CL_0000039)
 * _Added_
    *  **+** [oocyte](http://purl.obolibrary.org/obo/CL_0000023) **SubClassOf** [female germ cell](http://purl.obolibrary.org/obo/CL_0000021)

### Changes for: [spicule center](http://purl.obolibrary.org/obo/PORO_0000188)

 * _Deleted_
    *  **-** [spicule center](http://purl.obolibrary.org/obo/PORO_0000188) **SubClassOf** ObjectExactCardinality( [adjacent to](http://purl.obolibrary.org/obo/sponge#adjacent_to) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [spicule center](http://purl.obolibrary.org/obo/PORO_0000188) **SubClassOf** ObjectExactCardinality( http://purl.obolibrary.org/obo/RO_0002220 [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [morphology](http://purl.obolibrary.org/obo/PATO_0000051)

 * _Deleted_
    *  **-** [morphology](http://purl.obolibrary.org/obo/PATO_0000051) **SubClassOf** [quality](http://purl.obolibrary.org/obo/PATO_0000001)
 * _Added_
    *  **+** [morphology](http://purl.obolibrary.org/obo/PATO_0000051) **SubClassOf** [physical object quality](http://purl.obolibrary.org/obo/PATO_0001241)

### Changes for: [hexactin](http://purl.obolibrary.org/obo/PORO_0000341)

 * _Deleted_
    *  **-** [hexactin](http://purl.obolibrary.org/obo/PORO_0000341) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [hexactin](http://purl.obolibrary.org/obo/PORO_0000341) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [hexaster](http://purl.obolibrary.org/obo/PORO_0000343)

 * _Deleted_
    *  **-** [hexaster](http://purl.obolibrary.org/obo/PORO_0000343) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [hexaster](http://purl.obolibrary.org/obo/PORO_0000343) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [follicle cell](http://purl.obolibrary.org/obo/PORO_0000320)

 * _Deleted_
    *  **-** [follicle cell](http://purl.obolibrary.org/obo/PORO_0000320) **SubClassOf** [adjacent to](http://purl.obolibrary.org/obo/sponge#adjacent_to) **some** [oocyte](http://purl.obolibrary.org/obo/CL_0000023)
 * _Added_
    *  **+** [follicle cell](http://purl.obolibrary.org/obo/PORO_0000320) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002220 **some** [oocyte](http://purl.obolibrary.org/obo/CL_0000023)

### Changes for: [amphitriaene](http://purl.obolibrary.org/obo/PORO_0000117)

 * _Deleted_
    *  **-** [amphitriaene](http://purl.obolibrary.org/obo/PORO_0000117) **SubClassOf** [has part](http://purl.obolibrary.org/obo/BFO_0000051) **some** [rhabd](http://purl.obolibrary.org/obo/PORO_0000500) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [cladome](http://purl.obolibrary.org/obo/PORO_0000207) ) 
 * _Added_
    *  **+** [amphitriaene](http://purl.obolibrary.org/obo/PORO_0000117) **SubClassOf** [has part](http://purl.obolibrary.org/obo/BFO_0000051) **some** [rhabd](http://purl.obolibrary.org/obo/PORO_0000500) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [cladome](http://purl.obolibrary.org/obo/PORO_0000207) ) 

### Changes for: [paucispicular fiber](http://purl.obolibrary.org/obo/PORO_0000447)

 * _Deleted_
    *  **-** [paucispicular fiber](http://purl.obolibrary.org/obo/PORO_0000447) **SubClassOf** ObjectMinCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [megasclere](http://purl.obolibrary.org/obo/PORO_0000098) ) 
 * _Added_
    *  **+** [paucispicular fiber](http://purl.obolibrary.org/obo/PORO_0000447) **SubClassOf** ObjectMinCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [megasclere](http://purl.obolibrary.org/obo/PORO_0000098) ) 

### Changes for: [pentactin](http://purl.obolibrary.org/obo/PORO_0000449)

 * _Deleted_
    *  **-** [pentactin](http://purl.obolibrary.org/obo/PORO_0000449) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
    *  **-** [pentactin](http://purl.obolibrary.org/obo/PORO_0000449) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [pentactin](http://purl.obolibrary.org/obo/PORO_0000449) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
    *  **+** [pentactin](http://purl.obolibrary.org/obo/PORO_0000449) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [tetractin](http://purl.obolibrary.org/obo/PORO_0000586)

 * _Deleted_
    *  **-** [tetractin](http://purl.obolibrary.org/obo/PORO_0000586) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [tetractin](http://purl.obolibrary.org/obo/PORO_0000586) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [biogenic silica](http://purl.obolibrary.org/obo/CHEBI_64389)

 * _Deleted_
    *  **-** [biogenic silica](http://purl.obolibrary.org/obo/CHEBI_64389) **SubClassOf** [chemical entity](http://purl.obolibrary.org/obo/CHEBI_24431)
 * _Added_
    *  **+** [biogenic silica](http://purl.obolibrary.org/obo/CHEBI_64389) **SubClassOf** [biogenic mineral](http://purl.obolibrary.org/obo/CHEBI_64391)
    *  **+** [biogenic silica](http://purl.obolibrary.org/obo/CHEBI_64389) **SubClassOf** [hydrated silica](http://purl.obolibrary.org/obo/CHEBI_64393)
    *  **+** [biogenic silica](http://purl.obolibrary.org/obo/CHEBI_64389) *[label](http://www.w3.org/2000/01/rdf-schema#label)* biogenic silica

### Changes for: [tetractine](http://purl.obolibrary.org/obo/PORO_0000587)

 * _Deleted_
    *  **-** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
    *  **-** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **EquivalentTo** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
    *  **+** [tetractine](http://purl.obolibrary.org/obo/PORO_0000587) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [spongin](http://purl.obolibrary.org/obo/PORO_0000029)

 * _Deleted_
    *  **-** [spongin](http://purl.obolibrary.org/obo/PORO_0000029) **SubClassOf** [secreted by](http://purl.obolibrary.org/obo/sponge#secreted_by) **some** [spongocyte](http://purl.obolibrary.org/obo/PORO_0000013)
 * _Added_
    *  **+** [spongin](http://purl.obolibrary.org/obo/PORO_0000029) **SubClassOf** http://purl.obolibrary.org/obo/RO_0003001 **some** [spongocyte](http://purl.obolibrary.org/obo/PORO_0000013)

### Changes for: [diaene](http://purl.obolibrary.org/obo/PORO_0000257)

 * _Deleted_
    *  **-** [diaene](http://purl.obolibrary.org/obo/PORO_0000257) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 
 * _Added_
    *  **+** [diaene](http://purl.obolibrary.org/obo/PORO_0000257) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [clad](http://purl.obolibrary.org/obo/PORO_0000206) ) 

### Changes for: [diactin](http://purl.obolibrary.org/obo/PORO_0000255)

 * _Deleted_
    *  **-** [diactin](http://purl.obolibrary.org/obo/PORO_0000255) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 
 * _Added_
    *  **+** [diactin](http://purl.obolibrary.org/obo/PORO_0000255) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [spicule ray](http://purl.obolibrary.org/obo/PORO_0000045) ) 

### Changes for: [diactine](http://purl.obolibrary.org/obo/PORO_0000256)

 * _Deleted_
    *  **-** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **EquivalentTo** [megasclere](http://purl.obolibrary.org/obo/PORO_0000098) **and** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
    *  **-** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **SubClassOf** ObjectExactCardinality( [has part](http://purl.obolibrary.org/obo/BFO_0000051) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
 * _Added_
    *  **+** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **EquivalentTo** [megasclere](http://purl.obolibrary.org/obo/PORO_0000098) **and** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 
    *  **+** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **SubClassOf** ObjectExactCardinality( [has component](http://purl.obolibrary.org/obo/RO_0002180) [actine ray](http://purl.obolibrary.org/obo/PORO_0000106) ) 

### Changes for: [sclerocyte](http://purl.obolibrary.org/obo/PORO_0000011)

 * _Deleted_
    *  **-** [sclerocyte](http://purl.obolibrary.org/obo/PORO_0000011) **SubClassOf** [secretes](http://purl.obolibrary.org/obo/sponge#secretes) **some** [spicule](http://purl.obolibrary.org/obo/PORO_0000017)
 * _Added_
    *  **+** [sclerocyte](http://purl.obolibrary.org/obo/PORO_0000011) **SubClassOf** http://purl.obolibrary.org/obo/RO_0003000 **some** [spicule](http://purl.obolibrary.org/obo/PORO_0000017)

### Changes for: [subatrial spicule](http://purl.obolibrary.org/obo/PORO_0000568)

 * _Deleted_
    *  **-** [subatrial spicule](http://purl.obolibrary.org/obo/PORO_0000568) **SubClassOf** [adjacent to](http://purl.obolibrary.org/obo/sponge#adjacent_to) **some** [atrial skeleton](http://purl.obolibrary.org/obo/PORO_0000155)
 * _Added_
    *  **+** [subatrial spicule](http://purl.obolibrary.org/obo/PORO_0000568) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002220 **some** [atrial skeleton](http://purl.obolibrary.org/obo/PORO_0000155)

### Changes for: [spicule](http://purl.obolibrary.org/obo/PORO_0000017)

 * _Deleted_
    *  **-** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **SubClassOf** [secreted by](http://purl.obolibrary.org/obo/sponge#secreted_by) **some** [sclerocyte](http://purl.obolibrary.org/obo/PORO_0000011)
 * _Added_
    *  **+** [spicule](http://purl.obolibrary.org/obo/PORO_0000017) **SubClassOf** http://purl.obolibrary.org/obo/RO_0003001 **some** [sclerocyte](http://purl.obolibrary.org/obo/PORO_0000011)

### Changes for: [spongocyte](http://purl.obolibrary.org/obo/PORO_0000013)

 * _Deleted_
    *  **-** [spongocyte](http://purl.obolibrary.org/obo/PORO_0000013) **SubClassOf** [secretes](http://purl.obolibrary.org/obo/sponge#secretes) **some** [spongin](http://purl.obolibrary.org/obo/PORO_0000029)
 * _Added_
    *  **+** [spongocyte](http://purl.obolibrary.org/obo/PORO_0000013) **SubClassOf** http://purl.obolibrary.org/obo/RO_0003000 **some** [spongin](http://purl.obolibrary.org/obo/PORO_0000029)

### Changes for: [apopylar cell](http://purl.obolibrary.org/obo/PORO_0000140)

 * _Deleted_
    *  **-** [apopylar cell](http://purl.obolibrary.org/obo/PORO_0000140) **EquivalentTo** [sponge cell](http://purl.obolibrary.org/obo/PORO_0000000) **and** [surrounds](http://purl.obolibrary.org/obo/sponge#surrounds) **some** [apopyle](http://purl.obolibrary.org/obo/PORO_0000046)
    *  **-** [apopylar cell](http://purl.obolibrary.org/obo/PORO_0000140) **SubClassOf** [surrounds](http://purl.obolibrary.org/obo/sponge#surrounds) **some** [apopyle](http://purl.obolibrary.org/obo/PORO_0000046)
 * _Added_
    *  **+** [apopylar cell](http://purl.obolibrary.org/obo/PORO_0000140) **EquivalentTo** [sponge cell](http://purl.obolibrary.org/obo/PORO_0000000) **and** http://purl.obolibrary.org/obo/RO_0002221 **some** [apopyle](http://purl.obolibrary.org/obo/PORO_0000046)
    *  **+** [apopylar cell](http://purl.obolibrary.org/obo/PORO_0000140) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002221 **some** [apopyle](http://purl.obolibrary.org/obo/PORO_0000046)

### Changes for: [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990)

 * _Added_
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) **SubClassOf** [anatomical system](http://purl.obolibrary.org/obo/UBERON_0000467)
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) **SubClassOf** [develops from](http://purl.obolibrary.org/obo/RO_0002202) **some** [mesoderm](http://purl.obolibrary.org/obo/UBERON_0000926)
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) **SubClassOf** [mesoderm-derived structure](http://purl.obolibrary.org/obo/UBERON_0004120)
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* Anatomical system that has as its parts the organs concerned with reproduction.
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* Geschlechtsorgan
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* animal reproductive system
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* genital system
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* genitalia
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* organa genitalia
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* reproductive tissue
    *  **+** [reproductive system](http://purl.obolibrary.org/obo/UBERON_0000990) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* systemata genitalia

### Changes for: [mesohyl](http://purl.obolibrary.org/obo/PORO_0000002)

 * _Deleted_
    *  **-** [mesohyl](http://purl.obolibrary.org/obo/PORO_0000002) **SubClassOf** [adjacent to](http://purl.obolibrary.org/obo/sponge#adjacent_to) **some** [choanoderm](http://purl.obolibrary.org/obo/PORO_0000200)
    *  **-** [mesohyl](http://purl.obolibrary.org/obo/PORO_0000002) **SubClassOf** [adjacent to](http://purl.obolibrary.org/obo/sponge#adjacent_to) **some** [pinacoderm](http://purl.obolibrary.org/obo/PORO_0000043)
 * _Added_
    *  **+** [mesohyl](http://purl.obolibrary.org/obo/PORO_0000002) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002220 **some** [choanoderm](http://purl.obolibrary.org/obo/PORO_0000200)
    *  **+** [mesohyl](http://purl.obolibrary.org/obo/PORO_0000002) **SubClassOf** http://purl.obolibrary.org/obo/RO_0002220 **some** [pinacoderm](http://purl.obolibrary.org/obo/PORO_0000043)

# Report for properties


## ObjectProperty objects lost from source: 7

 * [surrounds](http://purl.obolibrary.org/obo/sponge#surrounds)
 * [null](http://www.w3.org/2002/07/owl#topObjectProperty)
 * [secretes](http://purl.obolibrary.org/obo/sponge#secretes)
 * [surrounded by](http://purl.obolibrary.org/obo/PORO_0000939)
 * [secreted_by](http://purl.obolibrary.org/obo/sponge#secreted_by)
 * [bearer of](http://purl.obolibrary.org/obo/BFO_0000053)
 * [null](http://purl.obolibrary.org/obo/sponge#adjacent_to)

## ObjectProperty objects new in target: 6


### New ObjectProperty : [has component](http://purl.obolibrary.org/obo/RO_0002180)

 * [has component](http://purl.obolibrary.org/obo/RO_0002180) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* For use in recording has_part with a cardinality constraint.
 * [has component](http://purl.obolibrary.org/obo/RO_0002180) *[label](http://www.w3.org/2000/01/rdf-schema#label)* has component
 * [has component](http://purl.obolibrary.org/obo/RO_0002180) *http://purl.obolibrary.org/obo/IAO_0000114* http://purl.obolibrary.org/obo/IAO_0000125
 * [has component](http://purl.obolibrary.org/obo/RO_0002180) *http://purl.obolibrary.org/obo/RO_0001900* http://purl.obolibrary.org/obo/RO_0001901

### New ObjectProperty : [null](http://purl.obolibrary.org/obo/RO_0002219)


### New ObjectProperty : [null](http://purl.obolibrary.org/obo/RO_0002220)


### New ObjectProperty : [null](http://purl.obolibrary.org/obo/RO_0002221)


### New ObjectProperty : [null](http://purl.obolibrary.org/obo/RO_0003001)


### New ObjectProperty : [null](http://purl.obolibrary.org/obo/RO_0003000)


## Changed ObjectProperty objects: 4


### Changes for: [capable of](http://purl.obolibrary.org/obo/RO_0002215)

 * _Deleted_
    *  **-** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[database cross reference](http://www.geneontology.org/formats/oboInOwl#hasDbXref)* RO:0002215
    *  **-** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[has obo namespace](http://www.geneontology.org/formats/oboInOwl#hasOBONamespace)* sponge
    *  **-** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[label](http://www.w3.org/2000/01/rdf-schema#label)* capable_of
    *  **-** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[shorthand](http://www.geneontology.org/formats/oboInOwl#shorthand)* capable_of
 * _Added_
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* A relation between a material entity (such as a cell) and a process, in which the material entity has the ability to carry out the process. 
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *[label](http://www.w3.org/2000/01/rdf-schema#label)* capable of
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000112* mechanosensory neuron capable of detection of mechanical stimulus involved in sensory perception (GO:0050974)
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000112* osteoclast SubClassOf 'capable of' some 'bone resorption'
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000114* http://purl.obolibrary.org/obo/IAO_0000125
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000117* Chris Mungall
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000118* has function realized in
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000119* PMID:20123131
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000119* PMID:21208450
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000232* For compatibility with BFO, this relation has a shortcut definition in which the expression "capable of some P" expands to "bearer_of (some realized_by only P)".
    *  **+** [capable of](http://purl.obolibrary.org/obo/RO_0002215) *http://purl.obolibrary.org/obo/IAO_0000424* RO_0000053 some (RO_0000054 only ?Y)

### Changes for: [develops from](http://purl.obolibrary.org/obo/RO_0002202)

 * _Deleted_
    *  **-** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[database cross reference](http://www.geneontology.org/formats/oboInOwl#hasDbXref)* RO:0002202
    *  **-** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[has obo namespace](http://www.geneontology.org/formats/oboInOwl#hasOBONamespace)* sponge
    *  **-** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[label](http://www.w3.org/2000/01/rdf-schema#label)* develops_from
    *  **-** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[shorthand](http://www.geneontology.org/formats/oboInOwl#shorthand)* develops_from
 * _Added_
    *  **+** ObjectPropertyDomain( [develops from](http://purl.obolibrary.org/obo/RO_0002202) [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) ) 
    *  **+** ObjectPropertyRange( [develops from](http://purl.obolibrary.org/obo/RO_0002202) [independent continuant](http://purl.obolibrary.org/obo/BFO_0000004) ) 
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* This is the transitive form of the develops from relation
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* x develops from y if and only if either (a) x directly develops from y or (b) there exists some z such that x directly develops from z and z develops from y
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *[label](http://www.w3.org/2000/01/rdf-schema#label)* develops from
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *http://purl.obolibrary.org/obo/IAO_0000114* http://purl.obolibrary.org/obo/IAO_0000125
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *http://purl.obolibrary.org/obo/IAO_0000117* Chris Mungall
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *http://purl.obolibrary.org/obo/IAO_0000117* David Osumi-Sutherland
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *http://purl.obolibrary.org/obo/IAO_0000117* Melissa Haendel
    *  **+** [develops from](http://purl.obolibrary.org/obo/RO_0002202) *http://purl.obolibrary.org/obo/IAO_0000117* Terry Meehan

### Changes for: [part_of](http://purl.obolibrary.org/obo/BFO_0000050)

 * _Deleted_
    *  **-** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[database cross reference](http://www.geneontology.org/formats/oboInOwl#hasDbXref)* BFO:0000050
    *  **-** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[has obo namespace](http://www.geneontology.org/formats/oboInOwl#hasOBONamespace)* sponge
    *  **-** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[label](http://www.w3.org/2000/01/rdf-schema#label)* part of
    *  **-** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[shorthand](http://www.geneontology.org/formats/oboInOwl#shorthand)* part_of
 * _Added_
    *  **+** InverseObjectProperties( [part of](http://purl.obolibrary.org/obo/BFO_0000050) [has part](http://purl.obolibrary.org/obo/BFO_0000051) ) 
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[label](http://www.w3.org/2000/01/rdf-schema#label)* part of
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *[label](http://www.w3.org/2000/01/rdf-schema#label)* part_of
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.obolibrary.org/obo/IAO_0000111* part of
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.obolibrary.org/obo/IAO_0000116* Intended meaning:
Ambiguous between continuant-parthood and occurrent-parthood.

domain: continuant
range: continuant
time: at some time

domain: occurrent
range: occurrent
time: atemporal
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.obolibrary.org/obo/IAO_0000116* Parthood as a relation between instances: The primitive instance-level relation p part_of p1 is illustrated in assertions such as: this instance of rhodopsin mediated phototransduction part_of this instance of visual perception.    This relation satisfies at least the following standard axioms of mereology: reflexivity (for all p, p part_of p); anti-symmetry (for all p, p1, if p part_of p1 and p1 part_of p then p and p1 are identical); and transitivity (for all p, p1, p2, if p part_of p1 and p1 part_of p2, then p part_of p2). Analogous axioms hold also for parthood as a relation between spatial regions.    For parthood as a relation between continuants, these axioms need to be modified to take account of the incorporation of a temporal argument. Thus for example the axiom of transitivity for continuants will assert that if c part_of c1 at t and c1 part_of c2 at t, then also c part_of c2 at t.    Parthood as a relation between classes: To define part_of as a relation between classes we again need to distinguish the two cases of continuants and processes, even though the explicit reference to instants of time now falls away. For continuants, we have C part_of C1 if and only if any instance of C at any time is an instance-level part of some instance of C1 at that time, as for example in: cell nucleus part_ of cell.
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.obolibrary.org/obo/IAO_0000118* part_of
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.obolibrary.org/obo/RO_0001900* http://purl.obolibrary.org/obo/RO_0001901
    *  **+** [part of](http://purl.obolibrary.org/obo/BFO_0000050) *http://purl.org/dc/elements/1.1/source* [OBO REL:part of](http://www.obofoundry.org/ro/#OBO_REL:part_of)

### Changes for: [has_part](http://purl.obolibrary.org/obo/BFO_0000051)

 * _Deleted_
    *  **-** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* Note that we relax the transitivity constraint of this relation to allow us to make cardinality axioms. This is not very satisfactory, in future versions we may use a sub-relation such as has-component'
    *  **-** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *[shorthand](http://www.geneontology.org/formats/oboInOwl#shorthand)* has_part
 * _Added_
    *  **+** InverseObjectProperties( [part of](http://purl.obolibrary.org/obo/BFO_0000050) [has part](http://purl.obolibrary.org/obo/BFO_0000051) ) 
    *  **+** TransitiveObjectProperty( [has part](http://purl.obolibrary.org/obo/BFO_0000051) ) 
    *  **+** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *[label](http://www.w3.org/2000/01/rdf-schema#label)* has_part
    *  **+** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *http://purl.obolibrary.org/obo/IAO_0000111* has part
    *  **+** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *http://purl.obolibrary.org/obo/IAO_0000116* Intended meaning:
Ambiguous between continuant-parthood and occurrent-parthood.

domain: continuant
range: continuant
time: at some time

domain: occurrent
range: occurrent
time: atemporal
    *  **+** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *http://purl.obolibrary.org/obo/IAO_0000118* has_part
    *  **+** [has part](http://purl.obolibrary.org/obo/BFO_0000051) *http://purl.obolibrary.org/obo/RO_0001900* http://purl.obolibrary.org/obo/RO_0001901
