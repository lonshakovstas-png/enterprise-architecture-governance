# REG-003: Architecture Dispute Management

| Field       | Value                                   |
| ----------- | --------------------------------------- |
| ID          | REG-003                                 |
| Status      | Approved                                |
| Version     | 1.0                                     |
| Date        | 2026-06-22                              |
| Author      | Digital Solutions Function              |
| Approved by | Head of Information Systems Development |
| Authority   | DOC-001                                 |

## Purpose

This process defines how disputes regarding architecture governance decisions, interpretations, compliance obligations, and governance artifact applicability are raised, reviewed, resolved, and recorded.

It provides a formal mechanism for resolving governance disagreements while maintaining consistency within the Enterprise Architecture Governance Framework.

## Scope

This process applies to disputes involving:

* Interpretation of approved governance artifacts
* Applicability of governance requirements
* Compliance obligations
* Architecture governance decisions
* Governance artifact conflicts

This process does not apply to:

* Governance artifact changes (governed by REG-001)
* Exception requests (governed by REG-002)

## Roles

| Role                                    | Responsibility                                  |
| --------------------------------------- | ----------------------------------------------- |
| Requestor                               | Raises dispute and provides supporting evidence |
| Responding Party                        | Provides response and supporting evidence       |
| Digital Solutions Function              | Reviews dispute and issues determination        |
| Head of Information Systems Development | Final escalation authority                      |

## Inputs

| Input                           | Required |
| ------------------------------- | -------- |
| Dispute Submission              | Yes      |
| Supporting Evidence             | Yes      |
| Governance Artifacts Referenced | Yes      |

A Dispute Submission shall include:

* Description of the dispute
* Parties involved
* Governance artifacts referenced
* Position of the Requestor
* Supporting evidence

## Process Flow

### 1. Submission

The Requestor submits a Dispute Submission to the Digital Solutions Function.

### 2. Review

The Digital Solutions Function reviews:

* Relevant governance artifacts
* Supporting evidence
* Positions of affected parties
* Authority hierarchy implications

### 3. Determination

The Digital Solutions Function issues one of the following determinations:

* Requirement applies
* Requirement does not apply
* Governance artifact interpretation clarified
* Governance conflict identified requiring change under REG-001

The determination shall be documented.

### 4. Escalation

If a party disputes the determination, the matter may be escalated to the Head of Information Systems Development.

### 5. Final Decision

The Head of Information Systems Development issues the final decision.

The final decision is binding.

## Outputs

| Output                           | Description                |
| -------------------------------- | -------------------------- |
| Determination                    | Initial dispute resolution |
| Escalated Decision               | Final binding decision     |
| Governance Change Recommendation | Referral to REG-001        |

## Escalation Rules

* Escalation shall occur only after a determination has been issued.
* The Head of Information Systems Development acts as final decision authority.
* Final decisions shall be recorded.

## Related Documents

* DOC-001 — Corporate Architecture and Architecture Governance Policy
* REG-001 — Architecture Change Management
* REG-002 — Architecture Exception Management
