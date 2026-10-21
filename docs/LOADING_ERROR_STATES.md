# Loading and Error States

Represent data-fetching states distinctly:

- loading while a request is pending,
- success with data,
- success with no matching data,
- recoverable request failure,
- unauthorized or unavailable data.

Avoid stale values that look like a successful refresh. Provide retry actions only when retrying is safe, and make error messages useful without exposing internal details.