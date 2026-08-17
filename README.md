# KOT3 — Hugo Blox Academic

Website for **Koopman Operator Theory: Fundamentals, Approximations and Applications 3**, held December 11–13, 2026 at Kyoto University.

Published site: <https://y-susuki.github.io/kot3/>

The site uses the official [Hugo Blox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) template and keeps its content in Markdown/YAML.

## Requirements

- Hugo Extended 0.162.0 or newer
- Go 1.19 or newer
- Node.js 22 or newer
- pnpm

## Local preview

```bash
pnpm install
pnpm dev
```

Open <http://localhost:1313/>.

## Production build

```bash
pnpm build
```

The generated static site is written to `dist/`.

## Editing content

- `content/_index.md` — homepage sections, dates, venue, sponsors, and contact information
- `data/authors/*.yaml` — organizing committee profiles
- `config/_default/menus.yaml` — navigation
- `config/_default/params.yaml` — identity, colors, header, and footer
- `assets/css/custom.css` — KOT3 visual customization
- `assets/media/sharing.png` — social sharing image

Hugo Blox configuration is pinned in `go.mod`, `go.sum`, and `hugoblox.yaml`.

Pushes to `main` are built and deployed automatically with GitHub Actions.
