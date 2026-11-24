# Tags Selection Motion Animation

An interactive motion prototype for choosing tools. Chips fly between a suggestion list and a selected field, change into a pastel color when they land, and pack back into the list when they are removed.

Open `index.html` in a browser. No build step or dependencies.

```bash
python3 -m http.server 8891
```

Then visit [http://127.0.0.1:8891/](http://127.0.0.1:8891/).

## Interaction

- Click a tool in the list to add it to **MY TOOLS LIBRARY**.
- Click the × on a selected tool to remove it.
- The selected field spans the full width of the card. Tools wrap onto the next line when the row is full.
- The list below shrinks to fit the tools that are still available. When every tool is selected, that list disappears.

## Motion

Adding a tool lifts the chip, tilts it, and flies it into the field. The chip takes its pastel color as it lands. The remaining chips slide together to close the gap.

Removing a tool flies it to the **first** spot in the list below, fades the pastel back to gray, and drops the ×. The other chips shift to make room, and the list height follows the content so empty space does not stay behind.

## Tools

Each selected tool has its own pastel:

| Tool | Color |
| --- | --- |
| Figma | Peach |
| Cursor AI | Lavender |
| Claude Code | Sand |
| Framer | Pink |
| Adobe Creative Cloud | Rose |
| Figma Make | Lilac |
| GitHub | Sage |
| Vercel | Sky |
| Lovable | Mint |
| PostHog | Butter |
| JIRA | Blue |
| ProtoPie | Apricot |
| Maze | Periwinkle |
| User Testing.com | Seafoam |

## Files

`index.html` is the whole prototype: layout, motion, and interaction.
