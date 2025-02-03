# React Router Dom v6 Catch-All Route Warning

This repository demonstrates a common, yet subtle, warning encountered when using React Router v6's catch-all route (`<Route path="*" />`). The warning occurs even when the catch-all route is correctly functioning and intended to handle 404 scenarios.

The issue stems from the placement of the catch-all route within the route hierarchy. While it works as expected, it triggers a console warning suggesting it's improperly nested.

**Solution:**
The solution involves restructuring the routes to avoid unnecessary nesting, particularly of the catch-all route.

The improved version avoids the warning by ensuring the catch-all route is at the top level of the route hierarchy.