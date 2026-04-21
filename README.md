# Design Tokens Vault — JSON Design Tokens & Design Language Docs for Popular Websites & Apps

> A free, open-source collection of JSON design tokens **and human-readable design language documentation** extracted from popular websites and apps. Use them to build clones, prototypes, design systems, or feed AI tools with precise UI context.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Tokens](https://img.shields.io/badge/sites-20-green.svg)](#covered-sites)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## What Is This?

**Design Tokens Vault** gives you two complementary artifacts for each brand:

| Artifact | Format | Best for |
|----------|--------|----------|
| **Design Tokens** (`tokens/*.json`) | DTCG-compatible JSON | Code — CSS vars, Tailwind, Style Dictionary, Figma |
| **Design Language** (`designs/*.md`) | Human-readable Markdown | AI prompts, design briefs, UI spec reference |

Whether you're:
- Building a **website clone** or UI study
- Bootstrapping a **design system** with proven values
- Doing **competitive design research**
- Feeding **AI coding tools** (Claude, Cursor, Copilot) rich visual context
- Speeding up **Figma-to-code** workflows

...this repo gives you the raw design context in formats every tool understands.

---

## Repository Structure

```
design-tokens-vault/
├── tokens/          # DTCG JSON design tokens (one file per brand)
│   ├── stripe.json
│   ├── linear.json
│   └── ...
└── designs/         # Markdown design language docs (one file per brand)
    ├── stripe.md
    ├── linear.md
    └── ...
```

---

## Design Language Docs (`designs/*.md`)

Each `.md` file is a structured design brief covering:

- **Aesthetic** — overall visual personality and feel
- **Color Usage** — exact hex values for every role (bg, text, brand, state)
- **Typography** — font family, size scale, weight, line height per context
- **Spacing** — base unit, section gaps, component internal padding
- **Layout** — page structure, grid, column ratios
- **Components** — buttons, cards, inputs, modals — exact specs per component
- **Visual Patterns** — recurring design motifs, imagery style, iconography
- **Motion** — duration, easing, specific animation behaviors

### Use with AI tools

Paste a design doc into your AI prompt to give it full visual context:

```
You are building a Stripe-style UI. Here is the exact design language:

<paste contents of designs/stripe.md>

Now build a pricing card component using these exact values.
```

Works with Claude, ChatGPT, Cursor, Copilot, v0, Bolt, and any other AI that accepts text context.

### Use as a design spec

Reference it during a Figma build or when writing a component library. Every color, size, and spacing value is documented by use-case, not just by name.

---

## Design Tokens (`tokens/*.json`)

Each JSON file follows the [Design Tokens Community Group (DTCG)](https://tr.designtokens.org/format/) spec:

```json
{
  "color": {
    "brand": { "value": "#635BFF", "type": "color" },
    "background": { "value": "#FFFFFF", "type": "color" },
    "text-primary": { "value": "#0A2540", "type": "color" }
  },
  "typography": {
    "font-family": { "value": "\"Sohne\", system-ui, sans-serif", "type": "fontFamily" },
    "font-size-base": { "value": "16px", "type": "dimension" }
  },
  "spacing": {
    "sm": { "value": "8px", "type": "dimension" },
    "md": { "value": "16px", "type": "dimension" },
    "lg": { "value": "24px", "type": "dimension" }
  },
  "border-radius": {
    "sm": { "value": "4px", "type": "dimension" },
    "md": { "value": "8px", "type": "dimension" }
  },
  "shadow": {
    "card": { "value": "0 4px 16px rgba(0,0,0,0.08)", "type": "shadow" }
  }
}
```

---

## Covered Sites

| Site | Category | Tokens | Design Doc |
|------|----------|--------|------------|
| [Stripe](./tokens/stripe.json) | Fintech / Payments | Colors, Typography, Spacing, Shadows | [stripe.md](./designs/stripe.md) |
| [Linear](./tokens/linear.json) | Productivity / SaaS | Colors, Typography, Spacing, Radius | [linear.md](./designs/linear.md) |
| [Notion](./tokens/notion.json) | Productivity | Colors, Typography, Spacing | [notion.md](./designs/notion.md) |
| [Vercel](./tokens/vercel.json) | Developer Tools | Colors, Typography, Spacing, Shadows | [vercel.md](./designs/vercel.md) |
| [GitHub](./tokens/github.json) | Developer Tools | Colors, Typography, Spacing, Radius | [github.md](./designs/github.md) |
| [Airbnb](./tokens/airbnb.json) | Marketplace | Colors, Typography, Spacing | [airbnb.md](./designs/airbnb.md) |
| [Spotify](./tokens/spotify.json) | Music / Entertainment | Colors, Typography, Spacing | [spotify.md](./designs/spotify.md) |
| [Discord](./tokens/discord.json) | Communication | Colors, Typography, Spacing, Radius | [discord.md](./designs/discord.md) |
| [Slack](./tokens/slack.json) | Communication / SaaS | Colors, Typography, Spacing | [slack.md](./designs/slack.md) |
| [Figma](./tokens/figma.json) | Design Tools | Colors, Typography, Spacing | [figma.md](./designs/figma.md) |
| [Tailwind UI](./tokens/tailwindui.json) | UI Framework | Colors, Typography, Spacing, Radius | [tailwindui.md](./designs/tailwindui.md) |
| [Shopify](./tokens/shopify.json) | E-Commerce | Colors, Typography, Spacing | [shopify.md](./designs/shopify.md) |
| [Netflix](./tokens/netflix.json) | Streaming / Entertainment | Colors, Typography, Spacing | [netflix.md](./designs/netflix.md) |
| [Apple](./tokens/apple.json) | Consumer Tech | Colors, Typography, Spacing, Radius | [apple.md](./designs/apple.md) |
| [Google](./tokens/google.json) | Search / Productivity | Colors, Typography, Spacing | [google.md](./designs/google.md) |
| [Meta](./tokens/meta.json) | Social Media | Colors, Typography, Spacing | [meta.md](./designs/meta.md) |
| [X / Twitter](./tokens/twitter.json) | Social Media | Colors, Typography, Spacing | [twitter.md](./designs/twitter.md) |
| [Uber](./tokens/uber.json) | Mobility / Marketplace | Colors, Typography, Spacing | [uber.md](./designs/uber.md) |
| [Loom](./tokens/loom.json) | Video / SaaS | Colors, Typography, Spacing | [loom.md](./designs/loom.md) |
| [Framer](./tokens/framer.json) | Design Tools / No-Code | Colors, Typography, Spacing | [framer.md](./designs/framer.md) |

> More sites added regularly. [Request a site →](https://github.com/mozammal-hossain/design-tokens-vault/issues/new?template=site-request.md)

---

## Usage

### 1. Copy a token file directly

```bash
# JSON tokens
curl -O https://raw.githubusercontent.com/mozammal-hossain/design-tokens-vault/main/tokens/stripe.json

# Design language doc
curl -O https://raw.githubusercontent.com/mozammal-hossain/design-tokens-vault/main/designs/stripe.md
```

### 2. Use design docs as AI context

```bash
# Copy a design doc to clipboard (macOS)
cat designs/stripe.md | pbcopy

# Then paste into your AI tool's system prompt or context window
```

Combine both artifacts for maximum AI accuracy:

```
Here are the Stripe design tokens (JSON) and the full design language spec (Markdown).
Use both to generate pixel-perfect components.

<paste tokens/stripe.json>
<paste designs/stripe.md>
```

### 3. Use with Style Dictionary

```js
// config.js
module.exports = {
  source: ["tokens/stripe.json"],
  platforms: {
    css: {
      transformGroup: "css",
      buildPath: "build/css/",
      files: [{ destination: "variables.css", format: "css/variables" }]
    }
  }
};
```

### 4. Use with Figma Tokens Plugin

Import any `.json` file directly into the [Figma Tokens](https://www.figma.com/community/plugin/843461159747178978) plugin. Use the matching `.md` file as your component spec reference.

### 5. Use with Tailwind CSS

```js
// tailwind.config.js
const stripeTokens = require("./tokens/stripe.json");

module.exports = {
  theme: {
    extend: {
      colors: {
        brand: stripeTokens.color.brand.value,
      }
    }
  }
};
```

---

## Token Categories

| Category | Description |
|----------|-------------|
| `color` | Brand, background, text, border, and state colors |
| `typography` | Font family, size scale, line height, letter spacing, font weight |
| `spacing` | Margin and padding scale |
| `border-radius` | Corner radius values |
| `shadow` | Elevation / box shadow values |
| `z-index` | Layer order scale |
| `motion` | Duration and easing values (where available) |

---

## Contributing

Have a site you want to see? Found a token that's wrong or outdated?

1. Fork the repo
2. Add `tokens/<site-name>.json` following the DTCG structure above
3. Add `designs/<site-name>.md` covering all sections (Aesthetic, Color, Typography, Spacing, Layout, Components, Visual Patterns, Motion)
4. Open a PR with the site name and source in the description

See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines.

---

## FAQ

**Are these official design tokens?**
No. These are reverse-engineered from public websites and are not officially published by the companies. Use for reference, learning, and prototyping only.

**What's the difference between the JSON and the `.md` files?**
The JSON tokens are machine-readable values for use in code and tooling. The `.md` design language docs are human-readable specs optimized for AI context, design briefs, and component documentation. They complement each other — use both.

**How do I request a site?**
[Open an issue](https://github.com/mozammal-hossain/design-tokens-vault/issues/new) with the site name. Community votes move requests up the queue.

**What format are tokens in?**
DTCG-compatible JSON. Works with Style Dictionary, Figma Tokens plugin, Theo, and custom build pipelines.

---

## License

MIT — free for personal and commercial use. See [LICENSE](LICENSE).

---

## Keywords

design tokens, JSON design tokens, UI design tokens, design language, AI UI context, website clone design, design system reference, color palette JSON, CSS variables, Figma tokens, typography tokens, spacing tokens, Stripe design tokens, Notion design tokens, Linear design tokens, Vercel design tokens, open source design tokens
