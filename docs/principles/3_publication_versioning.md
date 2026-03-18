# 3. Publication and Versioning

## Summary
A versioning and publication workflow is mandatory.
It must document changes made, the date of publication, and the version number.
The workflow itself must also be documented and publicly accessible.

## Purpose
Ontologies change throughout their lifecycle, and users need to be aware when and
what changes have occurred. Since ontology changes are typically made incrementally
and infrequently, versioning provides the mechanism to distinguish between states of
an ontology over time. Publication ensures that new versions are findable and
accessible to all users and downstream systems.

## Implementation

### Versioning
- ENERO Foundry ontologies MUST use a versioning workflow that publishes new
  ontology versions and documents:
    - changes made in each version (e.g. as a changelog)
    - dates of version publication
    - version numbers
- Developers MAY use either a semantic versioning format (SemVer) or a calendar
  versioning format (CalVer). Guidance on the differences between these two formats
  can be found at https://glinteco.com/en/post/understanding-semver-vs-calver-making-the-right-choice-for-your-project/
- The annotation `owl:versionInfo` MUST be used to identify the version number.
- The annotation `owl:versionIRI` MUST be used to identify the versioned resource.
- The versioning workflow for each ontology MUST be documented
  and publicly available.

### Publication Locations
Ontologies SHOULD be published in at least one of the following locations,
with a persistent, stable IRI:
- A **version control platform** (e.g. GitHub, GitLab) — recommended as the
  primary development and release channel, as it supports changelogs, release
  tagging, and issue tracking.
- An **ontology repository or terminology service** (e.g. TIB Terminology Service,
  OLS) — recommended for discoverability within the broader ontology community.
- A **project or institute website** — acceptable as a secondary publication point,
  but must not be the sole location, as institutional URLs are less stable over time.

Regardless of location, the published IRI of an ontology MUST remain stable
across versions. Version-specific IRIs (via `owl:versionIRI`) MAY change between
releases, but the ontology's primary IRI MUST always resolve to the latest version.

### Publication Frequency
No fixed release schedule is mandated, as the appropriate frequency will vary
depending on the covered domain, the stage of development, and available resources.
However, ontology developers SHOULD:
- Communicate the expected maintenance status and release cadence in the
  ontology's documentation.
- Signal clearly if an ontology is in active development, maintenance-only mode,
  or no longer maintained.

Publication frequency is considered an indicator of active maintenance and is
implicitly linked to the **Collaboration and Responsiveness** principle: long
periods without releases or communication may indicate that an ontology is
outdated or no longer supported.
