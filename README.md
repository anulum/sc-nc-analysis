<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-ANALYSIS — repository foundation
-->

# SC-NC Analysis

SC-NC Analysis is being built as the analysis layer split out of SC-NeuroCore: the observable series taken from runs and recordings, their statistical summaries, and the fits, cohorts and measurements that compare models with data. It imports SC-NC Core, SC-NC Catalogue and SC-NC Engine. This checkout contains repository validation tooling and documentation only. Full foundation qualification is in progress. There is no installed analysis package, statistics runner, model fitter or qualified record schema.

**What does not exist yet:**
- any code moved from SC-NeuroCore;
- a registered runtime record schema;
- an installed analysis package, statistics runner or model fitter.

## Boundary

**What this project owns:**

| Record | Scope |
|---|---|
| Observable series | A named observable over time, with its source run or recording and its sampling |
| Statistical summary | A statistic over one or more series, with its method, sample size and uncertainty |

**Schemas it takes over from SC-NeuroCore:** sc-neurocore.fit (v1 and v2), sc-neurocore.cohort (v1 and v2) and sc-neurocore.measurement (v1 and v2).

**Static imports:** only SC-NC Core, SC-NC Catalogue and SC-NC Engine.

**Records read without importing their code:** SC-NC Verify, SC-NC Bench, SC-NC Research, SC-NC Studio and Experiment Ledger read this repository's records.

**Records it reads without importing their code:** those of SC-NC Core, Spike Log, SC-NC Engine and SNN Divergence Harness.

**Code planned to move here from SC-NeuroCore,** package by package, when SC-NeuroCore's split import gate allows it: `analysis`, `autofit`, `fitting`, `spike_train_statistics`, `stochastic_doctor`, `explain`, `explainability`, `debug` and `topology`.

**Explicit non-claims and operating boundaries:**
- It contains no simulator and no trainer; it analyses runs and recordings.
- A statistic states its method, sample and uncertainty; it is not a finding beyond them.

## Current tooling

Repository controls inspect:
- metadata and source attribution;
- workflows and dependency alignment;
- native documentation and repository inventory;
- preflight orchestration.

Metadata declares architecture-only maturity with empty implemented domain capability and claim inventories.

- Use the exact environment in [Contributing](CONTRIBUTING.md).
- Full CI and preflight belong in CI or in an explicitly admitted pre-push environment.
- See [Validation](VALIDATION.md) for the maintained validation scope.

## Intended evidence

Every future record will carry its source and environment digests, its numeric formats where it has them, and its explicit verification boundary. None of the planned record schemas is registered or qualified by this foundation.

## Documentation and support

Read [Architecture](ARCHITECTURE.md), [support](SUPPORT.md), [security reporting](SECURITY.md) and [citation metadata](CITATION.cff).

**Not claimed:**
- a hosted service, released package or DOI;
- a public CI status;
- a performed simulation, hardware measurement or benchmark result.

## Licence

Source is licensed under [AGPL-3.0-or-later](LICENSE). A commercial licence is available through the contact in [NOTICE](NOTICE.md).

![ANULUM](docs/assets/anulum_logo_company.jpg)

![Fortis Studio](docs/assets/fortis_studio_logo.jpg)

## Text and data mining reservation
The rightsholder, Miroslav Šotek (ANULUM), expressly reserves the use of the
works in this repository for text and data mining, including the collection of
this content for, and its use in, training, fine-tuning or evaluating machine
learning and artificial intelligence models, in accordance with Article 4(3) of
Directive (EU) 2019/790 and the national provisions transposing it.

No permission for such use has been granted beyond what the licence in
`LICENSE` grants. This reservation does not change that licence: uses the
licence permits remain permitted on its terms, including its attribution and
share-alike conditions.

Reservation made on 2026-11-22. Requests for permission: contact the
rightsholder through the contact listed in this repository.
