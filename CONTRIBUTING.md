# Contributing

Thank you for improving the Enfoque Pest Control website. Keep changes focused, easy to review, and grounded in a clear visitor or business outcome.

## Set up the project

Use Node.js 24 and npm 11:

```bash
nvm use
npm ci
npm run dev
```

## Make a change

1. Create a short branch from the latest `main`.
2. Follow Conventional Commits for branch context, commits, and the pull request title.
3. Keep unrelated cleanup out of the change.
4. Update documentation when behavior, tooling, or workflow changes.

Examples:

```text
feat(landing): add commercial service proof
fix(header): preserve icon rendering on iOS
docs: clarify local setup
```

## Product and implementation guidelines

- Write visitor-facing content in clear Mexican Spanish.
- Keep code, comments, commits, and repository documentation in English.
- Prefer semantic HTML and native browser behavior.
- Preserve keyboard navigation, visible focus, useful alternative text, and sufficient contrast.
- Test layouts on narrow mobile, tablet, and desktop viewports.
- Keep the site static and avoid client-side JavaScript unless the interaction requires it.
- Use local, optimized assets when possible. Do not commit unlicensed third-party media.
- Treat contact destinations as configurable channels; avoid coupling interface copy to a provider unless the product requires it.
- Add `rel="noopener noreferrer"` to external links opened in a new tab.
- Never commit generated output from `dist/` or `.astro/`.

## Validate locally

Run the same quality gate used in continuous integration:

```bash
npm run check
```

The repository does not currently have an automated browser or unit-test suite. Do not add placeholder tests merely to satisfy a metric; introduce a test runner with the first behavior that benefits from durable automated coverage.

## Open a pull request

- Use a Conventional Commits title.
- Complete the English pull request template.
- Explain the problem, scope, validation, and production impact.
- Include screenshots or a preview for visible changes.
- Confirm that no secrets, credentials, or customer information are present.

## Security

Report vulnerabilities privately through the repository's GitHub Security Advisories instead of opening a public issue.
