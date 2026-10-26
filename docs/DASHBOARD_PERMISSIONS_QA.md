# Dashboard Permissions QA

Verify that dashboard data follows the application's access rules.

- Test with representative roles, not only an administrator.
- Check that restricted records are not exposed through charts or totals.
- Confirm filters cannot bypass server-side authorization.
- Distinguish an empty authorized result from an access error.
- Recheck permissions after role or data-model changes.

UI visibility is not a substitute for server-side access control.