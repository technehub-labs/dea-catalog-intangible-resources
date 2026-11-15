# CR-INR-CAT-03: IntangibleResource Candidate Corpus

**Status**: Landed (this PR)
**Layer**: Catalog content (candidate corpus intake)
**Owner**: Emmanuel A. Otchere
**Date**: 2026-11-16
**Admission authority**: candidate corpus only (canonical admission remains the evidence-gated step; FOUNDATIONS D-4/D-5)
**Trigger**: Skeleton-advance wave continuation (2026-11 owner directive): advance the remaining kit skeletons with evidence-backed candidate corpora. Intangible-resources: the SPDX License List + OSI approved licenses (published license registries) are the candidate seed sources; protection_type=license matches the entity enum directly.
**Carrier**: Single PR on feature branch `feat/cr-inr-cat-03`. PR review, not direct push.
**Lands against**: `main`
**Depends on**: INR-CAT-02 (ingestion groundwork).

## 1. What this CR lands

**740 IntangibleResource candidate submissions** in `contributions/queue/<shard>/<slug>.yaml` from 1 evidence bank(s):

| Bank | Source | Records |
|---|---|---|
| spdx-osi-licenses.json | SPDX License List + OSI approved licenses (published license registries) | 740 |

Provenance in `ingestion/manifest.yaml` (bank sha256s, source URLs, retrieval dates, mapping note). Every submission carries `source_ref`, a `published-document` evidence citation, and published description prose. Provisional field mappings are documented per record and in the manifest; per-organization values are canonical-admission decisions.


## 2. What changes

- `contributions/queue/<shard>/` — 740 intake submissions (`status: queued`)
- `ingestion/manifest.yaml` — corpus provenance record (new)
- No `CATALOG.yaml` change (queue ≠ index)
- This CR file and the index row

## 3. Verification

- `check_contributions.py`: CONFORMANT (740 queue files)
- No directory holds 800+ entries (slug-prefix distribution)
- Spot-checks: records trace to their published source identifiers

## 4. NOT-List

- NOT record admission (nothing under `entities/` changes; admission follows in INR-CAT-04+).
- NOT a modification of gates, schemas, or intake tooling.
- NOT an authoritative assessment of provisional mapped values.

## 5. Acceptance criteria

1. 740 gate-CONFORMANT submissions; manifest carries bank sha256s + source URLs.
2. Submissions carry no `id`; `status: queued`; `submitted_by: Emmanuel A. Otchere`.
3. `CATALOG.yaml` counts unchanged.
