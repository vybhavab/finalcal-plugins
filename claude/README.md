# FinalCal for Claude

Find events, check availability, and create, edit, or delete Google Calendar
events using your FinalCal account. This plugin connects to FinalCal's hosted
MCP server and includes a calendar workflow. It runs no local server and bundles
no credentials. It requires a FinalCal account with a linked Google account.

After the backend is deployed, upload `finalcal-claude-0.1.0.zip` in Claude's
Customize → Plugins → Add → Upload plugin flow. Enable FinalCal and use the
connection flow to sign in and approve access on FinalCal's connect page.
If the host asks for the connector URL, use `https://finalcal.com/mcp` with OAuth.
Read access is sufficient to inspect calendars; choose write access to change
events. Host and workspace policies may control plugin availability.

Try “What is on my calendar tomorrow?” or “Find a free half-hour for me and
alex@example.com next week.” Specify the calendar and time zone for scheduling.
Inviting guests may send email. Series IDs affect an entire recurring series.
Connections expire after 30 days and can be disconnected immediately at
https://finalcal.com/mcp/connections.

Documentation: https://finalcal.com/docs/mcp/
Support: https://finalcal.com/support/
Privacy: https://finalcal.com/privacy/
Terms: https://finalcal.com/terms/

The MIT license covers this distribution package only. The hosted FinalCal
service remains subject to its terms. Installing a package does not publish a
directory listing. Public source: https://github.com/vybhavab/finalcal-plugins
(folder `claude`, branch `main`). Publishing guide:
https://claude.com/docs/plugins/submit
