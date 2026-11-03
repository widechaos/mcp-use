# Inspector RPC panel keyboard evidence

Recordings for mcp-use/mcp-use issue #3005, from the actual standalone Inspector connected to a synthetic local MCP server. Chromium runs headlessly on macOS at a desktop viewport. No account, API key, or remote provider is used.

- [Before](before.webm): native Tab enters an invisible control inside the collapsed RPC panel. The behavioral regression fails.
- [After](after.webm): the same traversal skips the collapsed panel.
- [Expanded controls](expanded-controls.webm): keyboard focus reaches the panel controls; search/filter state survives closing and reopening, and the open preference survives reload.

The source remains mounted; only its inert state follows the open switch. Tests inspect native activeElement and layout geometry. These recordings do not establish screen-reader speech or other browser-engine behavior.
