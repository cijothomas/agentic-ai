KAW Agentic AI course contents

## Slides

The course deck uses [Slidev](https://sli.dev/). The 12-slide introduction in
`slides.md` covers AI foundations, LLMs, prompts, agents, tools, RAG, search,
protocols, frameworks, and agent architecture.

The deck was converted from the supplied [Google Slides presentation](https://docs.google.com/presentation/d/1xSpnpqlJkiJ5g5Tb6Kf8ubTxwY5AUhGLZJiMEJaPXU4/edit).
Text is editable in `slides.md`; shared layouts and colors are in `style.css`.
The four original illustrations are retained in `public/images/` with descriptive
alternative text. The conversion preserves the source's wording and slide order.
PDF animations and speaker notes are not included.

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
