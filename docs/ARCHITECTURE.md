<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-ANALYSIS — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Observable series | A named observable over time, with its source run or recording and its sampling | Source digests and sampling checks |
| Statistical summary | A statistic over one or more series, with its method, sample size and uncertainty | The method and sample are declared before the statistic is computed |

## Planned record schemas

- `sc_nc_analysis.observable_series.v1`
- `sc_nc_analysis.statistical_summary.v1`

These are planned identifiers. None of them is registered or qualified here.

It also takes over, unchanged, sc-neurocore.fit (v1 and v2), sc-neurocore.cohort (v1 and v2) and sc-neurocore.measurement (v1 and v2) from SC-NeuroCore when their code moves here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
