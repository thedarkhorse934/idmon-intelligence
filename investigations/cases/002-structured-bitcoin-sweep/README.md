# Investigation 002 — Structured Bitcoin Sweep and Consolidation

On 30 July 2026, a selected structural cohort of **1,195 Bitcoin transactions** moved value from **2,350 source outpoints** into **four repeated destination scripts** over blocks 960183–960191.

The case was reconstructed from retained local Bitcoin Core evidence and then compared against IDMON's previously saved blind-replay decisions.

### What happened

- 1,195 first-stage transactions converged on four repeated destinations containing 104, 100, 491 and 500 sweeps.
- Gross first-stage input was **1,082.65318922 BTC**.
- First-stage fees totalled **0.06638490 BTC**.
- Three verified consolidation transactions later spent 1,036 collector outputs.
- At the recorded 18 October 2026 snapshot, three consolidation outputs plus 159 residual collector outputs remained unspent.
- Terminal traced value was **1,082.56919591 BTC**.
- Exact accounting reconciled with an unreconciled difference of **0 satoshis**.

### What IDMON surfaced

In the saved replay:

- **0 / 1,195** selected first-stage sweeps surfaced;
- all first-stage transactions were recorded `INELIGIBLE` under the saved 100 BTC eligibility rule;
- **2 / 3** consolidation transactions surfaced;
- the remaining consolidation was also below the saved 100 BTC threshold.

The result exposes a specific difference between **transaction scale** and **episode scale**: individually sub-threshold transactions can collectively form a large structured flow.

### Research implication

The case supports further research into **threshold-independent detection of sweep-to-collector episodes**. That capability is a research direction only; it was not implemented or validated by this investigation.

### What we cannot establish

The retained evidence does **not** establish:

- a common controller across all four destinations;
- legal or beneficial ownership;
- purpose or motive;
- theft or compromise;
- device or entity attribution;
- whether the movement represented an economic sale.

### Evidence status

The reconstruction is explicitly bounded to the disclosed structural cohort and block range. Cohort selection was exploratory rather than a pre-registered detector test, and the replay comparison is a retrospective comparison against saved decisions.

## Full report

📄 **[Read Investigation Report 002 — Structured Bitcoin Sweep and Consolidation](./IDMON_Investigation_Report_002_Structured_Bitcoin_Sweep_V1.pdf)**

## Methodology

IDMON investigations classify findings as:

`ON_CHAIN_FACT` · `IDMON_EXISTING_LABEL` · `OBSERVED_PATTERN` · `HEURISTIC_INFERENCE` · `UNRESOLVED`

See the full [Evidence Standards](../../methodology/evidence-standards.md).
