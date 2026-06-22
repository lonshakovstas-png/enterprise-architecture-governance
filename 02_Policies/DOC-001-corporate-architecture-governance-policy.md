# DOC-001: Corporate Architecture and Architecture Governance Policy

| Field       | Value                      |
|-------------|----------------------------|
| ID          | DOC-001                    |
| Status      | Approved                   |
| Version     | 1.0                        |
| Date        | 2026-06-22                 |
| Author      | Digital Solutions Function |
| Approved by | Head of Information Systems Development |
| Authority   | ADR-0011                   |

## Purpose

This policy establishes the governance obligations, principles, and authority
framework for corporate architecture within the Digital Solutions function.

It mandates the use of the Enterprise Architecture Governance Framework as the
governing instrument for all architectural decisions, policies, processes, and
standards within scope. It defines the document authority hierarchy under which
all architecture governance artifacts operate and sets compliance requirements
that apply to all parties within scope.

## Scope

This policy applies to the Digital Solutions function and all initiatives,
projects, decisions and changes affecting the corporate information system.

It applies to all architecture governance artifacts produced, maintained, or
relied upon within that scope, regardless of the team or organisational unit
producing them.

## Provisions

### Governance Principles

**P-01 — Governed decision-making**

Architecturally significant decisions shall be formally recorded as ADRs.

**P-02 — Single source of truth**

The enterprise-architecture-governance repository is the primary authoritative
source for all architecture governance artifacts. Artifacts not maintained in
the repository are not considered part of the governance baseline.

**P-03 — Authority hierarchy**

Architecture governance documents operate under a fixed authority hierarchy.
Higher-level documents take precedence over lower-level documents in cases of
conflict:

ADR > DOC > REG > STD

**P-04 — Mandatory compliance**

Compliance with the governance framework is mandatory for all parties within
scope. Exceptions require a formally documented and approved process.

**P-05 — Framework continuity**

The governance framework shall be maintained as the organisation evolves.
Changes to the framework structure shall be introduced through a new or
superseding ADR.

### Canonical Document Types

All architecture governance artifacts shall conform to one of the four canonical
document types defined by the framework:

| Type | Purpose |
|------|---------|
| ADR | Architecture Decision Records — binding decisions |
| DOC | Policies and Charters — governance intent |
| REG | Governance Procedures — internal process definition |
| STD | Standards — normative specifications |

Supporting artifact types — Templates, Registers, and Glossary — operate in
support of the canonical types and are maintained in the repository accordingly.

### Document Compliance Requirements

All parties within scope shall:

- Record architecturally significant decisions as ADRs prior to implementation
- Maintain policies and charters as DOC documents in conformance with the approved DOC template
- Define governance processes as REG documents before operationalisation
- Maintain normative technical and process specifications as STD documents
- Use approved document templates when producing governance artifacts
- Maintain all governance artifacts in the enterprise-architecture-governance repository

No governance artifact shall be considered authoritative unless it is present
in the repository with Status: Approved.

## Responsibilities

### Digital Solutions Function

The Digital Solutions Function is responsible for:

- Maintaining the Enterprise Architecture Governance Framework
- Maintaining the enterprise-architecture-governance repository
- Approving Minor Amendments in accordance with REG-001
- Ensuring governance artifacts remain consistent with the approved baseline

### Head of Information Systems Development

The Head of Information Systems Development is responsible for:

- Executive accountability for the architecture governance function
- Formal approval of New Artifacts
- Formal approval of Major Revisions
- Formal approval of Supersessions
- Formal approval of Withdrawals
- Final escalation authority for governance decisions

### All Parties Within Scope

All teams, projects, and initiatives within scope are responsible for:

- Complying with this policy and all documents in the authority hierarchy
- Producing governance artifacts in conformance with approved document types and templates

## Review

This policy shall be reviewed semi-annually from its approval date, or upon any
change to the Enterprise Architecture Governance Framework structure,
whichever occurs first.

| Field | Value |
|--------|--------|
| Review Cycle | Semi-Annual |
| Next Review Date | 2026-12-22 |
| Review Authority | Digital Solutions Function |