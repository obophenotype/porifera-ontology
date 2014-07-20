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
 * VersionIRI: http://purl.obolibrary.org/obo/poro/releases/2014-03-07/poro.owl

# Report for classes


## Class objects lost from source: 0


## Class objects new in target: 1


### New Class : [fusiform](http://purl.obolibrary.org/obo/PORO_0001000)

 * [fusiform](http://purl.obolibrary.org/obo/PORO_0001000) *[definition](http://purl.obolibrary.org/obo/IAO_0000115)* Shape of a monactin spicule, tapering regularly toward an end.
 * [fusiform](http://purl.obolibrary.org/obo/PORO_0001000) *[label](http://www.w3.org/2000/01/rdf-schema#label)* fusiform
 * [fusiform](http://purl.obolibrary.org/obo/PORO_0001000) **SubClassOf** [morphology](http://purl.obolibrary.org/obo/PATO_0000051)

## Changed Class objects: 6


### Changes for: [monaxonic megasclere](http://purl.obolibrary.org/obo/PORO_0000412)

 * _Deleted_
    *  **-** [monaxon](http://purl.obolibrary.org/obo/PORO_0000412) *[label](http://www.w3.org/2000/01/rdf-schema#label)* monaxon
 * _Added_
    *  **+** [monaxonic megasclere](http://purl.obolibrary.org/obo/PORO_0000412) *[has related synonym](http://www.geneontology.org/formats/oboInOwl#hasRelatedSynonym)* monaxon
    *  **+** [monaxonic megasclere](http://purl.obolibrary.org/obo/PORO_0000412) *[label](http://www.w3.org/2000/01/rdf-schema#label)* monaxonic megasclere

### Changes for: [monactine](http://purl.obolibrary.org/obo/PORO_0002043)

 * _Deleted_
    *  **-** [monact](http://purl.obolibrary.org/obo/PORO_0002043) *[has exact synonym](http://www.geneontology.org/formats/oboInOwl#hasExactSynonym)* monactine
    *  **-** [monact](http://purl.obolibrary.org/obo/PORO_0002043) *[label](http://www.w3.org/2000/01/rdf-schema#label)* monact
 * _Added_
    *  **+** [monactine](http://purl.obolibrary.org/obo/PORO_0002043) *[has exact synonym](http://www.geneontology.org/formats/oboInOwl#hasExactSynonym)* monact
    *  **+** [monactine](http://purl.obolibrary.org/obo/PORO_0002043) *[label](http://www.w3.org/2000/01/rdf-schema#label)* monactine

### Changes for: [verticillate acanthostyle](http://purl.obolibrary.org/obo/PORO_0002005)

 * _Deleted_
    *  **-** [verticillated acanthostyle](http://purl.obolibrary.org/obo/PORO_0002005) *[label](http://www.w3.org/2000/01/rdf-schema#label)* verticillated acanthostyle
 * _Added_
    *  **+** [verticillate acanthostyle](http://purl.obolibrary.org/obo/PORO_0002005) *[label](http://www.w3.org/2000/01/rdf-schema#label)* verticillate acanthostyle

### Changes for: [acanthostyle](http://purl.obolibrary.org/obo/PORO_0002002)

 * _Added_
    *  **+** [acanthostyle](http://purl.obolibrary.org/obo/PORO_0002002) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* Subtypes of acanthostyle other than verticillate acanthostyle have yet to be named

### Changes for: [obsolete fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328)

 * _Deleted_
    *  **-** [fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) **SubClassOf** [monaxon](http://purl.obolibrary.org/obo/PORO_0000412)
    *  **-** [fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* Spicules of Demospongiae. Editors note: merge with oxea?
    *  **-** [fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[label](http://www.w3.org/2000/01/rdf-schema#label)* fusiform spicule
 * _Added_
    *  **+** [obsolete fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[comment](http://www.w3.org/2000/01/rdf-schema#comment)* Obsoleted as fusiform is better represented as a quality
    *  **+** [obsolete fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[deprecated](http://www.w3.org/2002/07/owl#deprecated)* true
    *  **+** [obsolete fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[label](http://www.w3.org/2000/01/rdf-schema#label)* obsolete fusiform spicule
    *  **+** [obsolete fusiform spicule](http://purl.obolibrary.org/obo/PORO_0000328) *[term replaced by](http://purl.obolibrary.org/obo/IAO_0100001)* PORO:0001000

### Changes for: [diactine](http://purl.obolibrary.org/obo/PORO_0000256)

 * _Deleted_
    *  **-** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **SubClassOf** [megasclere](http://purl.obolibrary.org/obo/PORO_0000098)
 * _Added_
    *  **+** [diactine](http://purl.obolibrary.org/obo/PORO_0000256) **SubClassOf** [monaxonic megasclere](http://purl.obolibrary.org/obo/PORO_0000412)

# Report for properties


## ObjectProperty objects lost from source: 0


## ObjectProperty objects new in target: 0


## Changed ObjectProperty objects: 0

