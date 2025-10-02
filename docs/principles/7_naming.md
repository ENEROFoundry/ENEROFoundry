# Identifier and Naming Conventions

## Description 
A consistent identifier format allows to understand where a class term is defined, helps in creating interoperable ontologies, and aids in the development of software that use the ontologies. Each entity in an ontology should therefore contain an identifier (IRI / CURIE) and a label. The identifier is used to identify the entity anywhere it is cited/used. The label is used as its main name / title.
## Requirements for labels (naming conventions)
- Use the annotation property rdfs:label for the primary label
- Each entity MUST have exactly one rdfs:label annotation
- labels MUST be unique within an ontology
- Synonyms/alternative labels can be added, e.g. via the annotation property IAO_0000118 (alternative term)
- Recommentation: 
    - write labels, synonyms, etc as if writing in plain English text. ie use spaces to separate words, only capitalize proper names (e.g. Parkinson disease). Do not use CamelCase, do_not_use_underscores. Avoid extra spaces between words, or at the beginning or end of the term labe
    - Spell out abbreviations. Abbreviations can be included as a separate property or synonym.
    - Make the primary labels to be as unambiguous as possible. Remember, your ontology may be used in a different context than that for which it was originally intended. Remember also of course that the label should be unambiguous without looking at parent terms
    - Avoid special characters like %, &, … in the mail label. They can be added for synonyms.

## Requirements for identifiers
Each entity MUST be given a unique IRI.
The usage of opaque identifiers is strongly recommended. This means that the IRI is an alpha-numeric identifier, in contrast to the natural language label. Tools like Ontology Lookup Services, Protégé etc. assist users with an automated translation to the human-readable label.

## Examples
### Labels and alternative labels / synonyms:
- rdfs:label "research and development grant",
- IAO_0000118 (alternative label) "research & development grant",
- IAO_0000118 (alternative label) "R&D grant"

### Identifiers:
- IRI: https://openenergyplatform.org/ontology/oeo/OEO_00360008 (energy balancing)
    - CURIE: [OEO:00360008](https://openenergyplatform.org/ontology/oeo/OEO_00360008)
- IRI: http://purl.obolibrary.org/obo/BFO_0000015 (process)
    - CURIE: [BFO:0000015](http://purl.obolibrary.org/obo/BFO_0000015)
