# Design Tokens Vault — JSON Design Tokens for Popular Websites & Apps

> A free, open-source collection of JSON design tokens extracted from popular websites and apps. Use them to build clones, prototypes, design systems, or reference UI when crafting pixel-perfect interfaces.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Tokens](https://img.shields.io/badge/sites-growing-green.svg)](#covered-sites)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## What Is This?

**Design Tokens Vault** provides structured JSON design tokens — colors, typography, spacing, border radius, shadows, and more — reverse-engineered from the world's most recognized digital products.

Whether you're:
- Building a **website clone** or UI study
- Bootstrapping a **design system** with proven values
- Doing **competitive design research**
- Speeding up **Figma-to-code** workflows

...this repo gives you the raw design context you need, in a format every tool understands.

---

## Token Structure

Each site ships a single JSON file following the [Design Tokens Community Group (DTCG)](https://tr.designtokens.org/format/) spec:

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

| Site | Category | Tokens |
|------|----------|--------|
| [Stripe](./tokens/stripe.json) | Fintech / Payments | Colors, Typography, Spacing, Shadows |
| [Linear](./tokens/linear.json) | Productivity / SaaS | Colors, Typography, Spacing, Radius |
| [Notion](./tokens/notion.json) | Productivity | Colors, Typography, Spacing |
| [Vercel](./tokens/vercel.json) | Developer Tools | Colors, Typography, Spacing, Shadows |
| [GitHub](./tokens/github.json) | Developer Tools | Colors, Typography, Spacing, Radius |
| [Airbnb](./tokens/airbnb.json) | Marketplace | Colors, Typography, Spacing |
| [Spotify](./tokens/spotify.json) | Music / Entertainment | Colors, Typography, Spacing |
| [Discord](./tokens/discord.json) | Communication | Colors, Typography, Spacing, Radius |
| [Slack](./tokens/slack.json) | Communication / SaaS | Colors, Typography, Spacing |
| [Figma](./tokens/figma.json) | Design Tools | Colors, Typography, Spacing |
| [Tailwind UI](./tokens/tailwindui.json) | UI Framework | Colors, Typography, Spacing, Radius |
| [Shopify](./tokens/shopify.json) | E-Commerce | Colors, Typography, Spacing |
| [Netflix](./tokens/netflix.json) | Streaming / Entertainment | Colors, Typography, Spacing |
| [Apple](./tokens/apple.json) | Consumer Tech | Colors, Typography, Spacing, Radius |
| [Google](./tokens/google.json) | Search / Productivity | Colors, Typography, Spacing |
| [Meta](./tokens/meta.json) | Social Media | Colors, Typography, Spacing |
| [X / Twitter](./tokens/twitter.json) | Social Media | Colors, Typography, Spacing |
| [Uber](./tokens/uber.json) | Mobility / Marketplace | Colors, Typography, Spacing |
| [Loom](./tokens/loom.json) | Video / SaaS | Colors, Typography, Spacing |
| [Framer](./tokens/framer.json) | Design Tools / No-Code | Colors, Typography, Spacing |

> More sites added regularly. [Request a site →](https://github.com/mozammal-hossain/your-design-context/issues/new?template=site-request.md)

---

## Usage

### 1. Copy a token file directly

```bash
curl -O https://raw.githubusercontent.com/mozammal-hossain/your-design-context/main/tokens/stripe.json
```

### 2. Use with Style Dictionary

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

### 3. Use with Figma Tokens Plugin

Import any `.json` file directly into the [Figma Tokens](https://www.figma.com/community/plugin/843461159747178978) plugin to apply tokens to your Figma file.

### 4. Use with Tailwind CSS

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
2. Add or update `tokens/<site-name>.json`
3. Follow the token structure above
4. Open a PR with the site name and source in the description

See [CONTRIBUTING.md](CONTRIBUTING.md) for full guidelines.

---

## FAQ

**Are these official design tokens?**
No. These are reverse-engineered from public websites and are not officially published by the companies. Use for reference, learning, and prototyping only.

**How do I request a site?**
[Open an issue](https://github.com/mozammal-hossain/your-design-context/issues/new) with the site name. Community votes move requests up the queue.

**What format are tokens in?**
DTCG-compatible JSON. Works with Style Dictionary, Figma Tokens plugin, Theo, and custom build pipelines.

---

## License

MIT — free for personal and commercial use. See [LICENSE](LICENSE).

---

## Keywords

design tokens, JSON design tokens, UI design tokens, website clone design, design system reference, color palette JSON, CSS variables, Figma tokens, typography tokens, spacing tokens, Stripe design tokens, Notion design tokens, Linear design tokens, Vercel design tokens, open source design tokens
