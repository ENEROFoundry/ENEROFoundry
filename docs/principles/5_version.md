# Versioning

## Summary
A versioning workflow that publishes newer ontology versions, documents changes made as well as the date of publication and version number, and documentation of this workflow, is mandatory.

## Purpose
Ontologies are expected to change during their lifecycle and users need to be aware that changes have occurred. However, it is assumed that changes to ontologies are made rather slowly. Versioning is therefore required to help distinguish which and when changes to an ontology have been made.

## Implementation
- OEO Foundry ontologies MUST use versioning workflows that publish newer ontology versions and document:
  - changes made in each version
  - dates of version publication
  - version numbers
- Documentation MUST be available for the versioning workflow of an OEOF ontology.
- Developers MAY use either a semantic versioning format or a calendaric versioning format. Information on the differences between these two format options can be found online, e.g. https://glinteco.com/en/post/understanding-semver-vs-calver-making-the-right-choice-for-your-project/.
- The annotation `owl:versionInfo` MUST be used to identify the version number of the ontology.
- The annotation `owl:versionIRI` MUST be used to identify the resource.
