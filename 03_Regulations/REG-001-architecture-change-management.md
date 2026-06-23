# REG-001: Architecture Change Management

| Field       | Value                                   |
| ----------- | --------------------------------------- |
| ID          | REG-001                                 |
| Status      | Approved                                |
| Version     | 1.1                                     |
| Date        | 2026-06-23                              |
| Author      | Digital Solutions Function              |
| Approved by | Head of Information Systems Development |
| Authority   | DOC-001                                 |

## Purpose

This process defines how governance artifacts within the Enterprise Architecture Governance Framework are created, amended, superseded, and withdrawn.

It operationalises the compliance requirements of DOC-001 and the framework continuity constraint of DOC-001 P-05: changes to the governance framework structure shall be introduced through a new or superseding ADR.

## Scope

This process applies to all changes to governance artifacts maintained in the enterprise-architecture-governance repository, including:

* Creation of new artifacts (ADR, DOC, REG, STD, Template, Register, Glossary entry)
* Minor amendments to existing artifacts
* Major revisions to existing artifacts
* Supersession of ADRs
* Withdrawal of artifacts

This process does not apply to:

* Exceptions to governance requirements (governed by REG-002)
* Operational project decisions below the threshold of architectural significance

## Roles

| Role                                    | Responsibility in this process                                                                             |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Proposer                                | Any party within scope who identifies a needed change to a governance artifact and prepares the submission |
| Digital Solutions Function              | Reviews all submissions; approves Minor Amendments; forwards other types to Head of ISD; implements        |
| Head of Information Systems Development | Approves New, Major Revision, Supersession, and Withdrawal; escalation authority for Minor Amendments      |

## Inputs

| Input                                        | Source   | Required / Optional                                 |
| -------------------------------------------- | -------- | --------------------------------------------------- |
| Change Proposal                              | Proposer | Required                                            |
| Draft artifact or revised artifact           | Proposer | Required for New, Minor, Major, Supersession        |
| Reference to existing artifact being changed | Proposer | Required for Minor, Major, Supersession, Withdrawal |
| Justification for withdrawal                 | Proposer | Required for Withdrawal only                        |

A Change Proposal shall state:

* The type of change (New / Minor Amendment / Major Revision / Supersession / Withdrawal)
* The governance artifact affected (for changes to existing artifacts)
* The rationale for the change

## Process Flow

### 1. Classification

The Proposer identifies the need for a governance artifact change and classifies it as one of the following types:

| Change Type     | Description                                                                              |
| --------------- | ---------------------------------------------------------------------------------------- |
| New             | A governance artifact that does not yet exist                                            |
| Minor Amendment | Editorial correction or clarification; no change to meaning, provisions, or requirements |
| Major Revision  | Substantive change to provisions, scope, or requirements                                 |
| Supersession    | An ADR is replaced by a new ADR; the existing ADR receives Status: Superseded            |
| Withdrawal      | An artifact is retired without replacement                                               |

### 2. Preparation

The Proposer prepares the submission according to the change type:

* **New:** Draft produced using the approved template for the artifact type (TPL-ADR, TPL-DOC, TPL-REG, or TPL-STD)
* **Minor Amendment** or **Major Revision:** Revised version of the existing artifact with changes clearly identifiable
* **Supersession:** Draft of the new superseding ADR; the new ADR shall reference the ADR it supersedes
* **Withdrawal:** No draft required; Change Proposal states the artifact to be withdrawn and the justification

### 3. Submission

The Proposer submits the Change Proposal and prepared artifact (where required) to the Digital Solutions Function.

### 4. Review

The Digital Solutions Function reviews the submission for:

* Correct use of the approved template
* Consistency with the document authority hierarchy (ADR > DOC > REG > STD)
* No conflict with existing approved artifacts in the governance baseline
* Correct change classification and versioning

### 5. Decision

The approval authority depends on the change type:

| Change Type     | Approval Authority                                                                                             |
| --------------- | -------------------------------------------------------------------------------------------------------------- |
| Minor Amendment | Digital Solutions Function                                                                                     |
| New             | Head of Information Systems Development, following review and recommendation by the Digital Solutions Function |
| Major Revision  | Head of Information Systems Development, following review and recommendation by the Digital Solutions Function |
| Supersession    | Head of Information Systems Development, following review and recommendation by the Digital Solutions Function |
| Withdrawal      | Head of Information Systems Development, following review and recommendation by the Digital Solutions Function |

The Digital Solutions Function reviews all submissions. For Minor Amendment submissions, the Digital Solutions Function approves or returns the submission directly. For all other change types, the Digital Solutions Function transmits its review finding and recommendation to the Head of Information Systems Development, who formally approves or returns the submission.

Returned submissions include documented reasons for return. Returned submissions restart at Step 2 upon resubmission.

### 6. Implementation

The Digital Solutions Function commits the approved change to the repository according to the change type:

| Change Type     | Repository Action                                                                           | Versioning                               |
| --------------- | ------------------------------------------------------------------------------------------- | ---------------------------------------- |
| New             | Artifact assigned canonical ID; Status set to Approved; committed to target directory       | Not applicable (first version)           |
| Minor Amendment | Revised artifact committed                                                                  | Minor version increment (e.g. 1.0 → 1.1) |
| Major Revision  | Revised artifact committed                                                                  | Major version increment (e.g. 1.0 → 2.0) |
| Supersession    | New ADR committed; original ADR updated to Status: Superseded with reference to new ADR     | ADRs are not versioned                   |
| Withdrawal      | Artifact moved to 99_Archive/ with suffix \_ARCHIVED-YYYY-MM-DD; Status updated to Withdrawn | No version change                        |

### Versioning Rules

* ADRs are not versioned.
* A change to an ADR always produces a new superseding ADR.
* DOC, REG and STD documents are versioned.
* Templates and Glossary entries do not carry version numbers.
* Registers carry a version number only when the register structure is formally revised.
* Operational updates to register contents (entry additions, updates or removals) do not constitute a version change.

## Outputs

| Output              | Location                                                          |
| ------------------- | ----------------------------------------------------------------- |
| Approved artifact   | Target directory in enterprise-architecture-governance repository |
| Superseded artifact | Original location; Status updated to Superseded                   |
| Archived artifact   | 99_Archive/                                                       |

## Escalation Rules

* If the Digital Solutions Function is unable to reach a decision on a Minor Amendment submission, the matter is escalated to the Head of Information Systems Development.
* The Head of Information Systems Development's decision is final and binding.
* All escalation decisions shall be documented in the affected governance artifact or associated change record.

## Related Documents

* DOC-001 — Corporate Architecture and Architecture Governance Policy
* ADR-0011 — Architecture Governance Framework v1.0
* REG-002 — Architecture Exception Management
* REG-003 — Architecture Dispute Management
