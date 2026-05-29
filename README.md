# mochi docs

This repo holds the source for the Mochi language documentation site at
[mochi-lang.dev](https://mochi-lang.dev).

It is automatically synced from the `website/` directory in
[mochilang/mochi](https://github.com/mochilang/mochi). Do not edit files
here by hand. Send changes to the main repo instead.

## What is here

- `docs/` - Markdown pages (manual, MEPs, research notes, implementation tracking)
- `src/` - React components and custom pages
- `static/` - Images and other static assets
- `docusaurus.config.js` - Site configuration
- `sidebars.js` - Navigation structure

## Local development

```sh
npm install
npm start
```

The site runs on `http://localhost:3000`.

## How the deploy works

Every push to `main` runs the `deploy.yml` workflow, which builds the site
with Docusaurus and deploys to Cloudflare Pages. The deploy is the only
workflow in this repo, so it never waits behind other CI jobs.

## License

MIT. See [LICENSE](LICENSE).
