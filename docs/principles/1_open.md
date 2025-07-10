# 1. Open

## Openness in OEO Foundry 

### Summary
**The ontology MUST be openly available to be used by all without any constraint** other than <br>
(a) acknowledgement of their origin and <br>
(b) it is not to be altered and subsequently redistributed in altered form under the original name or with the same identifiers.

### Purpose
OEO Foundry ontologies are resources intended for reuse and interoperability among energy-related domains and communities. 
An explicitly stated copyright license clearly stating the acceptable use reduces legal risks for users and promotes use and reuse. 
Therefore, the ontologies must be available to all without any constraint on their use or redistribution.

### Choice of license
OEO Foundry Ontologies MUST 
- be released under a **public domain** mark or **permissive open license**
- have an [OSI approved](https://opensource.org/licenses) or [open definition approved](https://opendefinition.org/licenses/api/) open license

Suitable open licenses
- Public domain under [Creative Commons CC0 1.0 Universal (CC0-1.0)](https://creativecommons.org/publicdomain/zero/1.0/legalcode.en) or equivalent.
- A permissive software license under [MIT License (MIT)](https://opensource.org/license/mit) or [BSD 3-Clause "New" or "Revised" License (BSD-3-Clause)](https://opensource.org/license/BSD-3-Clause) or equivalent.
- The use of a [Creative Commons Attribution 4.0 International (CC-BY-4.0)](https://creativecommons.org/licenses/by/4.0/legalcode.en) is possible but not recommended (see [discussion](https://opensource.stackexchange.com/questions/9242/why-does-creative-commons-recommend-not-using-cc-by-licenses-for-software)).

Recommendation: <br>
To reflect the dual nature of ontologies as both databases and software, we encourage to use the **dual license** “CC0 1.0 OR MIT” or equivalent.

The license MUST be clearly stated using the http://purl.org/dc/terms/license property followed by the URL representing the license (e.g. https://creativecommons.org/publicdomain/zero/1.0/legalcode.en) in the ontology file ([OWL example](https://oboacademy.github.io/obook/reference/formatting-license/)).

### Technical implementation: 
OEO Foundry ontologies MUST specify the reuse constraints using the `dcterms:license` annotation in any publicly released OWL version of the ontology. <br>
Example: <br>
`<dcterms:license rdf:datatype="&xsd;anyURI">[http://opensource.org/licenses/MIT</dcterms:license](http://opensource.org/licenses/MIT%3c/dcterms:license)>`

### Ontology re-use: 
Any ontology reusing individual terms from another ontology should
-	re-use the original terms IRI and 
-	use an `IAO:imported from` annotation http://purl.obolibrary.org/obo/IAO_0000412 on each imported term 
-	to link back to the group (i.e. ontology) maintaining it, where more information would be available about the license include any annotations for term or definition editors from the original ontology
