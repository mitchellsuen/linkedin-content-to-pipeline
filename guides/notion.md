# Set up your Notion content board

[Back to LinkedIn Content to Pipeline](../README.md)

Build a blank content board in your own Notion workspace from the schema bundled in this repo. Your agent records the resulting IDs in ignored `context/strategy/notion.local.json`, starting from [the example config](../context/strategy/notion.example.json).

## Build the board

Give your agent a destination page you own and paste:

```text
Use setup-workspace. Set up the blank content system under this Notion parent:
[MY PARENT PAGE URL]. Read context/strategy/notion-schema.md. Inspect the
parent first and reuse matching databases if present. Create or map Content
Board, Pillars & Topics, Hooks and Creator Inspo DB. Keep author-specific rows
empty until we define them. Store verified IDs in
context/strategy/notion.local.json. Verify the resulting schemas and tell me
which views or native templates, if any, still need a UI step.
```

The [schema](../context/strategy/notion-schema.md) and [page-body templates](../context/templates) are bundled.

| Database | Main fields |
|---|---|
| Content Board | Name, Status, Pillar, Platform, Publish date |
| Pillars & Topics | Name, Level, Pillar, Status, One line |
| Hooks | Hook, Type; the reusable pattern in the body |
| Creator Inspo DB | Full Name and platform URLs |

Use one pillar per piece. Store the paste-ready post in a text code block. Keep voice, source evidence and proof in the repo. Creator Inspo DB is optional.

Changing a date or status in Notion does not schedule a LinkedIn post. Review the exact copy, media, account and time in whatever scheduler you use. There is no bundled automatic sync from Notion to any publishing tool.
