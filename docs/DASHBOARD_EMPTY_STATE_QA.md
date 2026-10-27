# Dashboard Empty-State QA

Verify the dashboard distinguishes:

- loading,
- successful data with records,
- successful query with no matches,
- failed request,
- unauthorized or unavailable data.

Check that clearing filters restores the expected result set. Never show a successful zero count when the underlying request failed.