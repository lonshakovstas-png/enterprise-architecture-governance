# REG-002: Architecture Exception Management

| Field       | Value                                   |
| ----------- | --------------------------------------- |
| ID          | REG-002                                 |
| Status      | Approved                                |
| Version     | 1.0                                     |
| Date        | 2026-06-22                              |
| Author      | Digital Solutions Function              |
| Approved by | Head of Information Systems Development |
| Authority   | DOC-001                                 |

## Purpose

This process defines how exceptions to approved architecture governance requirements are requested, assessed, approved, recorded, reviewed, and retired.

It provides a controlled mechanism for temporary deviation from approved governance artifacts while preserving the integrity of the Enterprise Architecture Governance Framework.

## Scope

This process applies to requests for temporary exceptions to requirements contained in approved ADR, DOC, REG and STD artifacts.

This process does not apply to:

* Changes to governance artifacts themselves (governed by REG-001)
* Disputes regarding governance decisions (governed by REG-003)

## Roles

| Role                                    | Responsibility                                     |
| --------------------------------------- | -------------------------------------------------- |
| Requestor                               | Submits exception request and justification        |
| Digital Solutions Function              | Reviews, approves, rejects and monitors exceptions |
| Head of Information Systems Development | Escalation authority                               |

## Inputs

| Input                  | Required |
| ---------------------- | -------- |
| Exception Request      | Yes      |
| Business Justification | Yes      |
| Impact Assessment      | Yes      |
| Requested Duration     | Yes      |

An Exception Request shall identify:

* Governance artifact affected
* Requirement affected
* Reason compliance cannot currently be achieved
* Business impact
* Risk of approval
* Risk of rejection
* Requested duration

## Process Flow

### 1. Request

The Requestor submits an Exception Request.

### 2. Assessment

The Digital Solutions Function assesses:

* Governance impact
* Business impact
* Technical impact
* Risk exposure
* Duration appropriateness

### 3. Decision

The Digital Solutions Function may:

* Approve
* Approve with conditions
* Reject

All decisions shall be documented.

### 4. Recording

Approved exceptions shall be recorded in the designated exception register.

The record shall include:

* Exception identifier
* Approval date
* Expiry date
* Requestor
* Decision authority
* Conditions
* Status

### 5. Monitoring

Approved exceptions shall be periodically reviewed.

Expired exceptions shall be:

* Closed
* Renewed through a new request
* Replaced by a governance change under REG-001

## Outputs

| Output             | Description                    |
| ------------------ | ------------------------------ |
| Approved Exception | Temporary deviation authorised |
| Rejected Exception | Deviation denied               |
| Closed Exception   | Exception retired              |

## Escalation Rules

If the Digital Solutions Function cannot reach a decision, the matter shall be escalated to the Head of Information Systems Development.

The decision of the Head of Information Systems Development is final.

## Related Documents

* DOC-001 — Corporate Architecture and Architecture Governance Policy
* REG-001 — Architecture Change Management
* REG-003 — Architecture Dispute Management
