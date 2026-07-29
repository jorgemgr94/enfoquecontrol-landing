# Enfoque Pest Control

Static marketing website for Enfoque Pest Control in Monterrey, Mexico. The site helps visitors identify a pest-control need, understand the available services, and start a quotation conversation.

## Stack

- [Astro](https://astro.build/) 7
- TypeScript
- Plain CSS scoped to Astro components
- Static output

The project intentionally has no client-side framework or Tailwind dependency. Keep the browser payload small unless an interaction clearly requires JavaScript.

## Requirements

- Node.js 24
- npm 11

The expected versions are documented in `.nvmrc` and `package.json`.

## Local development

```bash
nvm use
npm ci
npm run dev
```

Astro serves the site at `http://localhost:4321` by default.

## Commands

| Command                | Purpose                                  |
| ---------------------- | ---------------------------------------- |
| `npm run dev`          | Start the local development server       |
| `npm run format`       | Format supported files with Prettier     |
| `npm run format:check` | Verify formatting without changing files |
| `npm run typecheck`    | Run Astro and TypeScript diagnostics     |
| `npm run build`        | Generate the production site in `dist/`  |
| `npm run preview`      | Preview the production build locally     |
| `npm run check`        | Run the complete local quality gate      |

## Project map

```text
src/
├── assets/       Local images processed by Astro
├── components/   Landing-page sections and reusable UI
├── layouts/      Shared document shell and metadata
└── pages/        Route entry points
public/           Files served without processing
```

No environment variables are required for the current static site.

## Delivery

Pull requests must use a [Conventional Commits](https://www.conventionalcommits.org/) title and pass formatting, type checking, and the production build. Dependabot checks npm and GitHub Actions dependencies monthly.

See [CONTRIBUTING.md](CONTRIBUTING.md) before making changes.
