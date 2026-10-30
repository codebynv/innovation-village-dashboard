# Dashboard Timezone Rules

For every timestamp shown in the dashboard, define:

- whether the stored value is UTC,
- which timezone is used for display,
- how date-only values are handled,
- which timezone controls daily and monthly aggregation,
- how daylight-saving changes are treated where relevant.

Keep chart buckets, filters, and displayed timestamps consistent. Verify with known timestamps near midnight before changing date calculations.