# Aspen

A landing page for **Aspen**, a fictional relationship-management app. This is
demo material for blog posts and video tutorials about AI-assisted design — a
deliberately "typical AI first pass" page, ready for you to improve along with
the tutorial.

Built with [Zola](https://www.getzola.org/) (static site generator) and
[Tailwind CSS v4](https://tailwindcss.com/).

## Prerequisites

- [Zola](https://www.getzola.org/documentation/getting-started/installation/)
- [Node.js](https://nodejs.org/) 18+ (or [Bun](https://bun.sh/))

## Getting started

```sh
npm install     # or: bun install
npm run dev     # compile CSS and watch for changes
```

Then in a second terminal:

```sh
zola serve      # serve the site at http://127.0.0.1:1111
```

## Production build

```sh
npm run build   # minified CSS + static site in public/
```

## Layout

```text
config.toml          # Zola site config
content/_index.md    # landing page frontmatter
templates/           # Tera templates (base shell + landing page)
src/input.css        # Tailwind entry point
static/              # favicon + compiled CSS output
```

## License

[MIT](LICENSE)
