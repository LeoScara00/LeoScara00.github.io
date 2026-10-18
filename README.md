# Leonardo Scaramelli — personal website

Academic website built with Astro, Tailwind CSS, MDX, and KaTeX.
Production address: https://leoscara00.github.io

## Run locally

Install Node.js 24 and pnpm 10, then run these commands in this folder:

```sh
pnpm install --frozen-lockfile
pnpm dev
```

Open the local address printed in the terminal. Saving a source file refreshes the preview.

## Where to make changes

- src/pages/: homepage, About, Research, and Explorations pages.
- src/components/FokkerPlanckPair.astro: interactive Ornstein–Uhlenbeck plots.
- src/components/ContactLinks.astro: contact links and icons.
- src/layouts/Layout.astro: shared header, footer, and theme switch.
- src/styles/global.css: colors, typography, and spacing.
- public/documents/: downloadable CV and thesis.
- examples/first-note.mdx: template for a future mathematical article.

## Publish updates

1. Edit and preview locally.
2. Run `pnpm build` to check the production build.
3. Commit the intended changes and push to main.
4. The Publish website workflow builds and deploys automatically.

The repository's Settings → Pages → Source must be set to GitHub Actions.
Only the generated dist folder is deployed; GitHub builds it from the source.
Dependencies, local backups, screenshots, and environment files are excluded from Git.

## Mathematical writing

Copy examples/first-note.mdx into src/pages/explorations/ with a descriptive filename.
Use dollar signs for inline mathematics and double dollar signs for display equations.
Add a link to the article in src/pages/explorations.astro.
