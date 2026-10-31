# Dashboard CSV Export QA

Before changing CSV export behavior, verify:

- exported rows match the active filters,
- column names are stable and meaningful,
- commas, quotes, and newlines are escaped correctly,
- text encoding is documented,
- empty results produce a valid, understandable file,
- sensitive fields are excluded,
- large exports have a defined limit or streaming strategy.

Open the downloaded CSV in a parser as well as a spreadsheet application.