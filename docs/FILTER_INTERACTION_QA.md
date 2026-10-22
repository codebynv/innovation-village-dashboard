# Filter Interaction QA

When reviewing dashboard filters, check:

- Each filter works independently.
- Multiple filters combine using the intended logic.
- Clearing a filter restores the expected dataset.
- Pagination resets or remains valid after filtering.
- Empty results are distinct from request errors.
- Displayed totals use the same filtered dataset as the chart.
- Refreshing the page handles query state consistently.

Use a small known dataset to confirm expected results.