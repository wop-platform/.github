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

## Multi-session & automated collaborators

Multiple automation sessions may share the same local checkouts of these
repositories. To keep that safe:

- **PR takeover must leave a trail**: if you close someone else's PR and reopen
  the work under a new branch/PR, you MUST comment on the original PR pointing
  to the new one before closing it.（接管他人 PR 必须先在原 PR 留言指向新 PR。）
- **No silent scope loss**: a takeover PR is only acceptable if the original
  PR's diff is fully contained in the new one — decisions confirmed in one PR
  (runtime floors, classifications, sentinels) must survive the handover.
  （验收条件：原 diff ⊆ 新 diff，已确认决议不得静默丢失。）
- **Never move another session's checkout**: do not switch, reset, or rebase a
  branch another session has checked out. Make your changes from an isolated
  `git worktree`, and push refs directly (`git push origin main:refs/heads/<b>`)
  when the shared checkout is occupied.
- **Verify against refs, not worktrees**: in shared checkouts the working tree
  can belong to anyone. Anchor all verification to git references
  (`git show <ref>:<path>`, `origin/main`) rather than on-disk files.
- **Diverged by rebased copies? realign, don't re-merge**: if `origin/main`
  contains rebased copies of your local commits (same content, different SHAs),
  reset your local branch to `origin/main` after confirming the content anchors
  match — never replay the originals on top.

## Reporting bugs & ideas

Use the issue templates (bug report / feature request) in the repository you found
the problem in. Include reproduction steps and environment details.
