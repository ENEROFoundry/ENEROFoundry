# Climate and Energy Policy Ontology (CEPO) — ENERO Principles Compliance

Assessment of the [Climate and Energy Policy Ontology](https://github.com/OpenEnergyPlatform/ontology) against the [ENERO Foundry Principles](https://enerofoundry.github.io/ENEROFoundry/principles/).

## Ontology Overview

**Ontology Name:** Climate and Energy Policy Ontology
**Abbreviation:** CEPO
**Homepage:** https://climatepolicyatlas.org/
**Primary Repository:** https://github.com/OpenEnergyPlatform/ontology
**Main Contact / Maintainer:** Amanda Wein (UOL) and Silvia Weko (FAU)

## Scope and Purpose

The CEPO is a collaborative effort between different researchers, from academia and
civil society, to map and clearly define different kinds of climate and
energy policy instruments.
The ontology is mainly used in the [Climate Policy Atlas](https://climatepolicyatlas.org/).
Existing ways of categorizing policy instruments in the climate and energy realm were
developed by practitioners like the International Energy Agency (IEA),
Organization for Economic Cooperation and Development (OECD),
[Climate Policy Database (CPDB)](https://climatepolicydatabase.org/)
and [Climate Policy Radar (CPR)](https://www.climatepolicyradar.org/).
These actors gather data on which policy documents have been published in certain years
and tag them with potential instruments.
However, their focus is mapping climate policies and their existence on a large scale,
not on the specific instruments and how they relate to each other.
In some cases, the methodology and definitions were not made publicly available.

We therefore propose a climate and energy policy ontology which encompasses instruments
at a sufficient level of detail to code in-depth policy data.
Rather than coding all “tax instruments” together, we differentiate between a
tax reduction, tax deduction, tax credit, tax exemption, and tax rebate
(all of which are types of tax incentives).
This level of granularity is important in being able to compare policies across
jurisdictions and time.
In order to ensure interoperability with other ontologies it makes use of the
Basic Formal Ontology (BFO) and its principles.
It also maps its alignment with the CPDB and CPR policy instrument typologies.

The ontology can be used to code policy documents with information about the
instruments that they contain.
Such policy data can be used to answer questions such as:

- Which countries tend to use the most regulatory instruments vs economic instruments to introduce electric vehicles?
- What are the most common types of tax incentives to promote renewable energy, and how have these changed over time?
- Which policy instruments (or mixes of policy instruments) have been the most effective at promoting decarbonization outcomes (emissions reductions, growth in clean energy generation, etc.)?

## Evaluation status legend

| Symbol | Meaning             |
|:------:|---------------------|
|   🟢   | Fully compliant     |
|   🟡   | Partially compliant |
|   ⚫    | Not yet implemented |
|   ⚪    | Not yet evaluated   |

## Compliance to ENERO Principles

# Climate and Energy Policy Ontology (CEPO) — ENERO Principles Compliance

Assessment of the [Climate and Energy Policy Ontology](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology) against the [ENERO Foundry Principles](https://enerofoundry.github.io/ENEROFoundry/principles/).

## Status legend

| Symbol | Meaning |
|:------:|---------|
| 🟢 | Fully met |
| 🟡 | Partially met — improvement recommended |
| ⚫ | Not yet implemented |

## Compliance table

|  #  | Principle                                                                                                   | Status | Assessment                                                                                                                                                                                                                                                                                                           | Key references                                                                                                                                                                                                                                                                                                                                            |
|:---:|-------------------------------------------------------------------------------------------------------------|:------:|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| P1  | [Openness](https://enerofoundry.github.io/ENEROFoundry/principles/1_open/)                                  |   🟢   | Dual-licensed CC0-1.0 or MIT (user's choice). License annotation property missing in the OWL file.                                                                                                                                                                                                                   | [LICENSE-CC0](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/LICENSE-CC0.txt) · [LICENSE-MIT](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/LICENSE-MIT.txt)                                                                                                                 |
| P2  | [Common Format](https://enerofoundry.github.io/ENEROFoundry/principles/2_format/)                           |   🟢   | Published in OWL format in `src/ontology/cepo.owl`. Uses standard OWL tooling consistent with OEO.                                                                                                                                                                                                                   | [Source](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/tree/production/src/ontology)                                                                                                                                                                                                                                               |
| P3  | [Release and Versioning](https://enerofoundry.github.io/ENEROFoundry/principles/3_release_versioning/)      |   🟢   | First initial release 0.1.1. `CHANGELOG.md` and `VERSION` file present. `RELEASE_PROCEDURE.md` documents the intended release process. `owl:versionInfo` status not yet verified against the OWL source.                                                                                                             | [CHANGELOG](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/CHANGELOG.md) · [RELEASE_PROCEDURE](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/RELEASE_PROCEDURE.md) · [VERSION](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/VERSION) |
| P4  | [Documentation](https://enerofoundry.github.io/ENEROFoundry/principles/4_documentation/)                    |   🟡   | README.rst, CONTRIBUTING.md, CODE_OF_CONDUCT.md, and CITATION.cff present. Used for the Climate Policy Atlas. Dedicated ontology documentation is missing.                                                                                                                                                           | [README](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/README.rst) · [Climate Policy Atlas](https://climatepolicyatlas.org/)                                                                                                                                                                                       |
| P5  | [Collaboration and Responsiveness](https://enerofoundry.github.io/ENEROFoundry/principles/5_collaboration/) |   🟢   | CONTRIBUTING.md and CODE_OF_CONDUCT.md present. GitHub Issues and PRs open and active (19 issues, 13 PRs). No regular developer meetings or formal community schedule.                                                                                                                                               | [CONTRIBUTING](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/CONTRIBUTING.md) · [Code of Conduct](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/CODE_OF_CONDUCT.md)                                                                                                         |
| P6  | [Scope](https://enerofoundry.github.io/ENEROFoundry/principles/6_scope/)                                    |   🟢   | Scope explicitly and carefully defined: climate and energy policy instruments, regulations, governance mechanisms. Includes explicit differentiation from existing databases (IEA, OECD, CPDB, CPR) and justification for the granularity of coverage. Clear statement of what CEPO adds beyond existing approaches. | [README](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/README.rst)                                                                                                                                                                                                                                                 |
| P7  | [Foundational Ontology](https://enerofoundry.github.io/ENEROFoundry/principles/7_foundation/)               |   🟢   | BFO alignment explicitly stated and the ontology makes use of the Basic Formal Ontology and its principles. Also maps alignment with the CPDB and CPR policy instrument typologies.                                                                                                                                  | [README](https://github.com/OpenEnergyPlatform/climate-energy-policy-ontology/blob/production/README.rst)                                                                                                                                                                                                                                                 |
| P8  | [Identifier and Naming Conventions](https://enerofoundry.github.io/ENEROFoundry/principles/8_naming/)       |   🟢   | No dedicated naming convention documentation found in the repository. IRI patterns follow OEO conventions (shared infrastructure with OEO) but are not formally specified. Recommendation: add naming convention guidelines to CONTRIBUTING.md.                                                                      | —                                                                                                                                                                                                                                                                                                                                                         |
| P9  | [Textual Definitions](https://enerofoundry.github.io/ENEROFoundry/principles/9_definitions/)                |   🟢   | Key classes defined in the scope section. Full coverage of classes and object properties not yet verified against the OWL source file. No automated definition tests found. Early-stage ontology.                                                                                                                    | —                                                                                                                                                                                                                                                                                                                                                         |
| P10 | [Usage of AI](https://enerofoundry.github.io/ENEROFoundry/principles/10_ai_usage/)                          |   ⚫    | No AI usage documentation found. Ontology is very new (first developed 2025). Principle may not yet have been applied or considered.                                                                                                                                                                                 | —                                                                                                                                                                                                                                                                                                                                                         |
