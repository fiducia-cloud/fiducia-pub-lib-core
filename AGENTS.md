# Fiducia public library agent instructions

- Work directly on `main` for now.
- Do not create feature branches or worktrees.
- Keep public APIs contract-first and aligned with `fiducia-interfaces`.
- Never commit credentials, plaintext environment files, generated build output,
  or host-specific paths.
- Run the repository checks before committing and push completed work to
  `origin/main`.
- If a non-main branch exists, merge it into `main` semantically, preserving
  compatible behavior from both sides; do not rebase or force-push.
