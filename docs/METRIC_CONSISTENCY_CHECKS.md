# Metric Consistency Checks

When validating dashboard metrics:

- Compare summary cards with the underlying filtered records.
- Verify charts and tables use the same filter state.
- Define how missing values affect calculations.
- Check rounding and displayed units.
- Distinguish unavailable data from a genuine zero.
- Verify refresh behavior and timestamps.

Use a small dataset with manually calculated expected values. Do not claim metric correctness without comparing actual results.