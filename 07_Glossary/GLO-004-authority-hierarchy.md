# GLO-004: Authority Hierarchy

| Field       | Value                                   |
|-------------|-----------------------------------------|
| ID          | GLO-004                                 |
| Status      | Approved                                |
| Date        | 2026-06-22                              |
| Author      | Digital Solutions Function              |
| Approved by | Head of Information Systems Development |

## Definition

The Authority Hierarchy is the precedence relationship between governance artifacts within the Enterprise Architecture Governance Framework.

Where two governance artifacts conflict, the artifact with the higher authority takes precedence.

The authority hierarchy is:

ADR > DOC > REG > STD

A lower-level artifact shall not contradict a higher-level artifact.

Where a conflict is identified, the lower-level artifact shall be revised, superseded, or withdrawn in accordance with REG-001.

## Interpretation

Authority hierarchy governs precedence only.

It does not imply ownership, organisational seniority, or approval authority.

## Supporting Artifacts

Templates, Registers, and Glossary entries are supporting artifacts.

They support the operation of the framework but do not participate in the authority hierarchy and carry no binding authority.

ADR-0011 §Decision describes supporting artifacts as operating below Standards, indicating their subordinate position relative to authoritative document types. This is equivalent in effect to their non-authoritative status.

## See Also

- [ADR-0011] §Decision
- [DOC-001] P-02 — repository authority principle
- [DOC-001] P-03 — authority hierarchy principle