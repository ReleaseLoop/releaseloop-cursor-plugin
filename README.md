# ReleaseLoop for Cursor

Connect Cursor to your [ReleaseLoop](https://releaseloop.com) account through the ReleaseLoop MCP server.

## What it does

The assistant works as you, so it can only see and change what your account can.

- Read workspaces, artists, releases, tasks, contacts, and royalty imports.
- List releases newest first, with an optional date range.
- Summarize one release: credits, tracks, tasks, marketing, and budget.
- Open a royalty import and summarize the rows that matched a release. It does not return the raw file.
- Create and update releases and tasks.

It cannot delete records or process payments. It will not change deal terms or file links.

If you belong to more than one workspace, name the one you mean. Sections you are not allowed to see (contacts, royalties, marketing, budget) are reported as hidden. Asking for the same release or task twice keeps the first one.

## Install

- From the Cursor Marketplace: search for ReleaseLoop once it is listed.
- From this repository: add `https://github.com/ReleaseLoop/releaseloop-cursor-plugin` as a Cursor plugin source.

After install, Cursor will ask you to sign in to ReleaseLoop. Review the permissions and click Allow connection. No API key is needed.

## Included

- `mcp.json`: the remote server at `https://mcp.releaseloop.com`
- `skills/plan-release`: inspect and plan a release
- `skills/manage-releases-tasks`: create and update releases and tasks
- `skills/royalties-contacts`: royalty imports and contacts

## Example prompts

- "Open my workspace, then list the scheduled releases. If I belong to more than one, stop and ask which workspace."
- "Open the release titled Night Bus. Summarize the tracks, open tasks, marketing, and budget. If marketing or budget isn't visible, say you don't have access."
- "Create a draft release titled Night Bus for artist Ada, out on 16 October 2026. Then try to create it again and tell me whether a copy was made."
- "On the Night Bus release, add a Marketing task called Pitch playlists. Leave it to do."
- "List my ReleaseLoop workspaces. Then list the contacts in the workspace I name. If contacts aren't accessible, say so and don't invent any."
- "Move the Night Bus release to Scheduled. Leave deal terms, owner share, and files alone."
- "Show the royalty imports in my workspace."

## Links

- Privacy policy: https://releaseloop.com/privacy
- Terms: https://releaseloop.com/terms
- MCP integration docs: https://docs.releaseloop.com/integrations/mcp/
- Example prompts: https://docs.releaseloop.com/integrations/mcp-prompts/

## License

MIT. See [LICENSE](LICENSE).
