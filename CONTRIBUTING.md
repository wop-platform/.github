# Contributing to wop-platform

Thanks for your interest in contributing! This is the organization-level default guide;
individual repositories may carry their own `CONTRIBUTING.md` with language-specific
conventions, which takes precedence.

## Ground rules for all repositories

- **Spec over implementation**: protocol behavior is defined by the public specs in
  [wop-specs](https://github.com/wop-platform/wop-specs). If you find a conflict between
  a spec and an implementation, open an issue first — never bend the spec to match
  existing code.
- **Golden vectors are read-only**: `crypto-vectors.json` is the cross-language
  byte-level conformance anchor. Proposals that modify vectors to make tests pass
  will be rejected; changes flow spec-first, then regenerate vectors.
- Keep public discussions in English or Chinese (中文 welcome).

## Workflow

1. Fork the repository and create a feature branch.
2. Make your change with tests; run the repository's own CI checks locally first
   (see each repo's `CONTRIBUTING.md`).
3. Open a Pull Request against `main` using the PR template.
4. Commits follow [Conventional Commits](https://www.conventionalcommits.org/)
   (Chinese bodies are fine).

## Reporting bugs & ideas

Use the issue templates (bug report / feature request) in the repository you found
the problem in. Include reproduction steps and environment details.
