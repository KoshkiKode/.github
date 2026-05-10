# Contributing to KoshkiKode Projects

Thanks for your interest in contributing! This guide applies across all KoshkiKode repositories: **Unshelv'd**, **Vetviona**, and **The Cordite Wars: Six Fronts**.

---

## Before You Start

- Check the open [issues](../../issues) and [pull requests](../../pulls) to make sure someone isn't already working on it.
- For significant changes, open an issue first to discuss the approach. This saves everyone time.
- All contributions are subject to the repository's `LICENSE` and, where applicable, the project `EULA.txt`.

---

## Development Setup

Each project has its own setup guide:

| Project | Setup Doc |
|---------|----------|
| Unshelv'd | `README.md` → Development section |
| Vetviona | `README.md` → Development section |
| Cordite Wars | `README.md` → Building from Source |

Always read the project-specific `README.md` before diving in.

---

## Branch Naming

```
feat/short-description       # new feature
fix/short-description        # bug fix
chore/short-description      # tooling, deps, cleanup
docs/short-description       # documentation only
refactor/short-description   # code change with no behaviour change
test/short-description       # adding or fixing tests
```

Branch off `main` unless told otherwise. Keep branches focused — one logical change per branch.

---

## Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short summary>

[optional body]

[optional footer]
```

**Types:** `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `perf`, `style`, `ci`

**Examples:**
```
feat(auth): add OAuth2 login via Google
fix(tree): prevent infinite loop on circular parent link
docs(deploy): update self-hosting guide for Caddy v2
chore: bump Flutter to 3.22
```

- Keep the summary under 72 characters.
- Use the imperative mood: "add feature", not "added feature".
- Reference issues in the footer: `Closes #42`

---

## Pull Requests

- Fill out the PR template completely — partial PRs will be asked to complete it.
- PRs should be small and focused. A PR that touches 20 unrelated files is hard to review.
- All CI checks must pass before a PR can be merged.
- At least one approving review is required (even as a solo dev, self-review via the checklist counts).
- Squash commits on merge for feature branches; merge commits for release branches.

---

## Code Style

| Project | Language | Formatter / Linter |
|---------|----------|-------------------|
| Unshelv'd | TypeScript | ESLint + Prettier (config in repo) |
| Vetviona | Dart | `dart format` + `flutter analyze` |
| Cordite Wars | C# | `.editorconfig` in repo root |

Run the formatter before committing. PRs with unformatted code will be asked to fix it.

---

## Reporting Bugs

Use the **Bug Report** issue template. Please include:
- Steps to reproduce (the more specific, the better)
- Expected vs actual behaviour
- Platform, OS version, app version
- Logs or screenshots if relevant

---

## Suggesting Features

Use the **Feature Request** issue template. Please include:
- What problem does this solve?
- Who benefits from it?
- Any alternatives you've considered?

---

## Security Issues

**Do not open a public issue for security vulnerabilities.** See [`SECURITY.md`](SECURITY.md) for the responsible disclosure process.

---

## Code of Conduct

Be respectful. Constructive criticism of code is welcome; personal attacks are not. We're all here to build something good.
