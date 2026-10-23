# Chart Data Validation

Before rendering chart data, check:

- values have the expected numeric type,
- missing values have a defined representation,
- category labels are stable and readable,
- totals agree with the underlying filtered dataset,
- empty datasets render an explicit empty state,
- large values and negative values are formatted correctly where supported.

Do not silently replace invalid values with zero unless that is the documented business rule.