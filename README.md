# Neat Icons MCP

Let your AI coding agent find icons and put them straight into your code.
Search 1,161 icons in 4 styles (Rounded Stroke, Rounded Solid, Sharp Stroke, Sharp Solid) and get each one as SVG, React or a data URI.

Hosted server, nothing to install:

```
https://mcp.neaticons.com/mcp
```

- **Free:** connect with no key. Your agent can search every icon, and the free icons come back as code.
- **Full set:** a Neat Icons license (Personal or Team) unlocks every icon plus animated icons. Get a seat key at [neaticons.com/activate](https://neaticons.com/activate) and send it as `Authorization: Bearer <seat key>`.

Website: [neaticons.com/mcp](https://neaticons.com/mcp)

## Connect

### Claude Code

```bash
claude mcp add --transport http neat-icons https://mcp.neaticons.com/mcp
```

### Cursor, Windsurf, VS Code and other clients

```json
{
  "mcpServers": {
    "neat-icons": {
      "url": "https://mcp.neaticons.com/mcp"
    }
  }
}
```

With a seat key, add a header:

```json
{
  "mcpServers": {
    "neat-icons": {
      "url": "https://mcp.neaticons.com/mcp",
      "headers": { "Authorization": "Bearer YOUR_SEAT_KEY" }
    }
  }
}
```

### ChatGPT

Add `https://mcp.neaticons.com/mcp` as a connector, with no authentication for the free icons.

## Tools

| Tool | What it does |
|---|---|
| `search_icons` | Find icons by name, tag or idea, across the whole set. Each result says if it is free. |
| `list_categories` | The categories in the set, with counts. |
| `get_icon` | One icon in a chosen style as SVG, a React component or a data URI, with size and color. Licensed keys can ask for the animated version. |
| `get_icons` | Several icons in one call. |

## Example prompts

- "Add a wallet icon to the checkout button, Rounded Stroke, 20px."
- "Find icons for a settings sidebar and give me React components."
- "Swap every icon on this page to Sharp Solid."

## Listed on

The official MCP Registry as `com.neaticons/icons`.

## Support

hello@djectstudio.com · Made by [DjectStudio](https://djectstudio.com)
