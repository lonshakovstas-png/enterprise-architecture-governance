# ADR-0011: Architecture Governance Framework v1.0

| Field | Value |
|---------|---------|
| ID | ADR-0011 |
| Status | Approved |
| Date | 2026-06-22 |

## Context

The Digital Solutions function lacked a formally defined Architecture Governance Framework. Architectural decisions were made without consistent documentation, document types were unstandardised, and no defined authority hierarchy governed the relationship between policies, procedures, and technical standards.

As the scope of architectural activity expanded, the absence of a framework introduced risk of:

- Inconsistent or conflicting architectural decisions
- Ungoverned exceptions to standards and policies
- No traceable record of governance obligations and their basis
- Ambiguity over which document type carried authority in cases of conflict

A framework was required to establish canonical document types, define their authority relationships, and provide a governed repository for all architecture governance artifacts.

## Decision

The Enterprise Architecture Governance Framework v1.0 is adopted.

The framework applies to the Digital Solutions function and all initiatives, projects, decisions and changes affecting the corporate information system.

The framework defines four canonical document types:

| Type | Purpose |
|------|---------|
| ADR | Architecture Decision Records — binding decisions |
| DOC | Policies and Charters — governance intent |
| REG | Governance Procedures — internal process definition |
| STD | Standards — normative specifications |

These types operate under a fixed authority hierarchy:

ADR > DOC > REG > STD

Supporting artifact types — Templates, Registers, and Glossary — operate below Standards. Higher-level documents take precedence over lower-level documents in cases of conflict.

All architecture governance artifacts are maintained in the enterprise-architecture-governance repository under the following structure:

- 01_ADR/ — Architecture Decision Records
- 02_Policies/ — Policies and Charters (DOC)
- 03_Regulations/ — Governance Procedures (REG)
- 04_Standards/ — Standards (STD)
- 05_Templates/ — Document Templates
- 06_Registers/ — Active Registers
- 07_Glossary/ — Terminology
- 99_Archive/ — Superseded and withdrawn documents

## Consequences

### Established

- Architectural decisions within scope are recorded and traceable
- A fixed authority hierarchy prevents conflicting governance artifacts
- Governance processes for change management, exception management and dispute management are formally defined as REG documents
- The repository provides a single source of truth for architecture governance

### Obligations

- Architectural decisions of framework scope must be documented as ADRs
- Policies and charters must conform to the DOC document type
- Governance processes must be defined as REG documents before implementation
- Technical and process specifications must be maintained as STD documents

### Constraints

- Framework artifacts require ongoing maintenance as the organisation evolves
- Changes to the Governance Framework structure shall be introduced through a new or superseding ADR
