# Repository guidance

Read `README.md` and `CONTRIBUTING.md` before changing the project. Treat scripts and configuration in the repository as the source of truth.

## Architecture

- This is a statically generated Astro site.
- Routes live in `src/pages`, the document shell in `src/layouts`, and page UI in `src/components`.
- Prefer scoped component styles and existing design tokens over global overrides.
- Keep visitor-facing copy in Spanish and repository artifacts in English.
- Avoid adding a client-side framework or JavaScript hydration for interactions that work with HTML and CSS.
- Store processed images in `src/assets`; use `public` only for assets that must retain an exact public path.
- Keep contact calls to action independent of any specific provider unless the requirement explicitly names one.

## Workflow

```bash
npm ci
npm run dev
npm run check
```

Run `npm run format` before the final validation when supported files change. Never commit `dist/`, `.astro/`, dependencies, secrets, credentials, or customer data.

## Delivery

- Branch from the latest `main`.
- Use Conventional Commits for commits and pull request titles.
- Keep each pull request focused on one outcome.
- Complete the pull request template in English.
- Include visual evidence for interface changes.
