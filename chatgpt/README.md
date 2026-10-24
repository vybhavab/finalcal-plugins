# FinalCal for ChatGPT and Codex

Find events, check availability, and manage events in Google calendars linked
to your FinalCal account. This package bundles a remote MCP connection, a
calendar workflow, icons, and proposed directory review cases. It contains no
OAuth client secret, access token, or Google credentials.

After deployment, use the OpenAI developer submission flow to upload
`finalcal-chatgpt-0.1.1.zip`. The public MCP URL is
`https://finalcal.com/mcp`. Authentication uses OAuth with automatic client
registration (DCR), S256 PKCE, and discovery. The default scope is
`calendar:read`; users can explicitly choose `calendar:write` on FinalCal's
connect page. Disconnect at https://finalcal.com/mcp/connections.

Try “What is on my calendar tomorrow?” or “Find a free hour next week.” Supply
the calendar and time zone for event changes. Invitations may email guests.
Availability can be unknown. New connections stay active until disconnected.
Connections made under the former 30-day policy require one reconnect to use the new policy. This package
does not contain an embedded calendar UI.

The `com.openai` authentication extension in `mcp.json` follows OpenAI's
packaging documentation. The upstream Agent Plugins 1.0.0 MCP schema currently
rejects that documented extension. The local build validates the portable
configuration and this narrowly defined OAuth extension separately; successful
OpenAI dashboard import is still required before submission.

The bundled review cases are proposed scenarios, not recorded host results.
Before submission, deploy and test the service, prepare a populated review
account, provide private review access through the dashboard, and add a real
demo recording URL. Never put review credentials in this ZIP.

Documentation: https://finalcal.com/docs/mcp/
Support: https://finalcal.com/support/
Privacy: https://finalcal.com/privacy/
Terms: https://finalcal.com/terms/

The MIT license covers this distribution package only. The hosted FinalCal
service remains subject to its terms. Public source:
https://github.com/vybhavab/finalcal-plugins (folder `chatgpt`). Publishing guide:
https://developers.openai.com/plugins/deploy/submission
