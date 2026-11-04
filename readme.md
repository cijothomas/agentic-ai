KAW Agentic AI course contents

## Slides

The course deck uses [Slidev](https://sli.dev/). The two hello-world slides in
`slides.md` are placeholders for the course material.

Published deck: <https://cijothomas.github.io/agentic-ai/>

## Local development

Use Node.js 24 (`nvm use` if you use nvm), then run:

```sh
npm ci
npm run dev
```

Open <http://localhost:3030> and edit `slides.md`. Separate slides with `---`.
Store future images and other static assets in `public/`.

## Build and publish

```sh
npm run build
```

The static site is generated in `dist/` with the `/agentic-ai/` base path required
by this repository's GitHub Pages URL.

The GitHub Actions workflow builds pull requests and deploys successful builds
from `main`. It can also be started manually from the Actions tab on `main`.
For initial setup, select **GitHub Actions** under **Settings → Pages → Build and
deployment → Source**. No deployment secret is needed; the workflow uses GitHub's
short-lived token and the `github-pages` environment.
