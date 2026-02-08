# Contributing

## Branch Conventions

- `main` — production-ready code
- `test/<feature>` — feature development and testing
- `fix/<issue>` — bug fixes
- `docs/<topic>` — documentation updates

**Never push directly to `main`.** All changes go through test branches and require review.

## Commit Format

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): description

[optional body]

[optional footer]
```

**Types:** `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `style`, `perf`, `ci`, `build`, `revert`

**Examples:**
```
feat(auth): add JWT refresh token rotation
fix(api): handle null response from payment provider
docs: update deployment instructions
chore(deps): bump next from 14.1.0 to 14.2.0
```

## Pull Request Process

1. Create a branch from `main`: `git checkout -b test/my-feature`
2. Make your changes with conventional commits
3. Push to your branch: `git push origin test/my-feature`
4. Open a PR against `main`
5. Fill in the PR template
6. Request review
7. Address feedback
8. Merge after approval (squash merge preferred)

## Code Style

- **Formatting**: Prettier (auto-formatted on commit via lint-staged)
- **Linting**: ESLint with project config
- **Types**: TypeScript strict mode

Run before committing:
```bash
npm run lint
npm run format:check
npm run typecheck
```

## Testing

- Write tests for new features and bug fixes
- Run `npm test` before pushing
- Maintain or improve code coverage

## Questions?

Open an issue or reach out to the maintainer.
