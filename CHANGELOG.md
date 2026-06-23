# Changelog

All notable changes to the Enterprise Architecture Governance Framework are documented here.

---

## [1.0.1] - 2026-06-23

### Corrected — Baseline Corrections

Post-baseline consistency corrections applied. All corrections are Minor Amendments approved by the Digital Solutions Function under REG-001.

#### DOC-001 v1.0 → v1.1

- Added Related Documents section referencing ADR-0011, DOC-002, REG-001, REG-002, REG-003, GLO-001 through GLO-004

#### DOC-002 v1.0 → v1.1

- Added Related Documents section referencing ADR-0011, DOC-001, REG-001, REG-002, REG-003, RGS-001

#### REG-001 v1.0 → v1.1

- Roles table: updated Digital Solutions Function and Head of ISD responsibilities to reflect tiered approval model
- Step 5 Decision: replaced single-authority approval with tiered approval table by change type
- Escalation Rules: scoped to Minor Amendment submissions; New, Major, Supersession, and Withdrawal go to Head of ISD as primary approver, not escalation
- Added REG-003 to Related Documents
- Versioning Rules promoted from bold emphasis to heading

#### REG-003 v1.0 → v1.1

- Step 3 Determination: added advisory language for disputes concerning a decision made by the Digital Solutions Function itself; either party may escalate directly under Step 4 without awaiting the Determination

#### RGS-001

- Updated versions: DOC-001 (1.1), DOC-002 (1.1), REG-001 (1.1), REG-003 (1.1); effective dates updated to 2026-06-23
- Corrected own-entry title from "Governance Artifact Register" to "Framework Artifact Register"

#### Repository documentation

- `README.md`: rewritten; corrected directory names (02_Policies, 03_Regulations, 04_Standards), removed duplicated content, added framework overview and navigation tables
- `STRUCTURE.md`: corrected directory names to include leading zeros (01_ADR, 02_Policies, etc.)

---

## [1.0.0] - 2026-06-23

### Baseline Complete

Enterprise Architecture Governance Framework v1.0 baseline is complete.
All 15 artifacts are imported, reviewed, and approved.

### Added — Commit 5: Register

- `RGS-001` — Framework Artifact Register: registers all 15 baseline artifacts (governance and supporting).

### Added — Commit 4: Glossary and Templates

- `GLO-001` — Architecturally Significant
- `GLO-002` — Governance Artifact
- `GLO-003` — Supersession (includes Status Vocabulary: Approved, Superseded, Withdrawn)
- `GLO-004` — Authority Hierarchy
- `TPL-ADR` — Architecture Decision Record Template
- `TPL-DOC` — Policy and Charter Template
- `TPL-REG` — Governance Procedure Template
- `TPL-STD` — Standard Template

### Added — Commit 3: Regulations

- `REG-001` — Architecture Change Management v1.0
- `REG-002` — Architecture Exception Management v1.0
- `REG-003` — Architecture Dispute Management v1.0

### Added — Commit 2: Policies

- `DOC-001` — Corporate Architecture and Architecture Governance Policy v1.0
- `DOC-002` — Digital Solutions Function Charter v1.0

### Added — Commit 1: Foundation

- `ADR-0011` — Architecture Governance Framework v1.0
- Repository structure: `01_ADR/`, `02_Policies/`, `03_Regulations/`, `04_Standards/`,
  `05_Templates/`, `06_Registers/`, `07_Glossary/`, `99_Archive/`
- `STRUCTURE.md`, `CHANGELOG.md`, `README.md`, `.gitignore`
