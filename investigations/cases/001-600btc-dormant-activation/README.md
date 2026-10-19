# Investigation 001 — 600 BTC Dormant-UTXO Activation

On 22 September 2026, IDMON detected the movement of approximately **600 BTC after ~14.2 years of dormancy**.

The economically material value came from **seven Bitcoin UTXOs created in July 2012**, which together totalled exactly **600 BTC**.

### What happened

- 35 inputs were consolidated into a single native-SegWit output.
- Roughly one hour later, the resulting ~600 BTC output was split into two near-equal ~300 BTC branches.
- One branch moved once more in the following block.
- At the Bitcoin Core tip checked for the investigation, both terminal outputs remained unspent.

### What we can establish

The report reconstructs the transaction path, exact UTXO accounting, dormancy, fees, script changes and downstream spends using retained IDMON evidence and read-only Bitcoin Core verification.

### What we cannot establish

The available evidence does **not** prove:

- who controlled the funds;
- whether beneficial ownership changed;
- why the BTC moved;
- whether a custodian or exchange was involved;
- whether the movement represented a sale.

This distinction between **confirmed blockchain evidence and analytical inference** is central to the IDMON Investigations methodology.

## Full report

📄 **[Read Investigation Report 001 — 600 BTC Dormant-UTXO Activation and Subsequent Split](./IDMON_Investigation_Report_001_600BTC_Dormant_Activation_V2.2.pdf)**

## Methodology

IDMON investigations classify findings as:

`ON_CHAIN_FACT` · `IDMON_EXISTING_LABEL` · `OBSERVED_PATTERN` · `HEURISTIC_INFERENCE` · `UNRESOLVED`

See the full [Evidence Standards](../../methodology/evidence-standards.md).
