# Change Requests: dea-catalog-intangible-resources

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-INR-CAT-01](CR-INR-CAT-01-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-INR-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-INR-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-INR-CAT-02](CR-INR-CAT-02-cr-inr-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-INR-CAT-02](CR-INR-CAT-02-cr-inr-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-INR-CAT-03](CR-INR-CAT-03-cr-inr-cat-03.md) | IntangibleResource Candidate Corpus | **Landed (this PR)** | 740 queue submissions from 1 bank(s); manifest with sha256s; queue gate CONFORMANT; no entities change. |
| [CR-INR-CAT-04](CR-INR-CAT-04-cr-inr-cat-04.md) | IntangibleResource Candidate Admission Batch 05 (BSD Zero Clause License (0BSD) … Zope Public License 2.1 (ZPL-2.1)) | **Landed (this PR)** | Admitted 740 `IntangibleResource` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +740, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
