# Julian Johnson — Master Inventory

A living dashboard of all tools, websites, systems, and content created across professional and personal areas.

## What's Inside

A single self-contained `index.html` file with three tabs:
- **📋 All Projects** — full catalog with expandable detail cards, category filters
- **⚡ Impact Summary** — cumulative hours saved per area and in total
- **🔧 Improvement Queue** — every suggested next step across all projects

## How to Host on GitHub Pages

1. Create a new GitHub repository (e.g. `inventory` or `operations-hub`)
2. Upload `index.html` and `README.md` to the root
3. Go to **Settings → Pages → Source: Deploy from branch → Branch: main → Folder: / (root)**
4. Your dashboard is live at `https://[your-username].github.io/[repo-name]/`

## How to Update

To add a new project or update an existing one, open `index.html` and find the `ITEMS` array near the top of the `<script>` block. Each project follows this structure:

```js
{
  id: "unique-id",
  category: "quiet-edge",    // quiet-edge | unified | personal | trading | content
  title: "Project Title",
  type: "Web Tool",          // Web Tool | Interactive Tool | Content | etc.
  status: "live",            // live | built | complete | in-progress | ongoing
  description: "Full description of what was built and why.",
  outputs: ["Output 1", "Output 2"],
  timeSaved: 10,
  timeSavedUnit: "hours of work",
  improvements: ["Improvement idea 1", "Improvement idea 2"],
  links: ["Link label or URL"],
  lastWorked: "May 2026",
}
```

To update the "Last updated" date in the footer, change the `LAST_UPDATED` constant at the top of the script.

## Areas Tracked

| Area | Description |
|---|---|
| 🏆 The Quiet Edge | Youth mental performance platform — video curriculum, web tools, content |
| 🎯 Unified Solutions | Executive coaching business — assessment, website, CRM, ICF tracking |
| 🏠 Personal & Financial | Home rental planning, debt strategy, income opportunities |
| 📈 Trading & Investing | NinjaTrader strategies, prop firm tools |
| ✍️ Content & Brand | LinkedIn posts, thought leadership content |

---

© Julian Johnson · Unified Solutions Inc. / The Quiet Edge
