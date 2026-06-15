# Git Hooks (shared)

These hooks are **shared with the team**. Activate once per clone:

```bash
git config core.hooksPath .githooks
```

## pre-commit

If you change `docs/*.mdx` but not `docs/updates.mdx` (the What's New log),
the commit prints a reminder. It **never blocks** the commit.

For notable doc additions/improvements, add an `<Update>` block to the top of
`docs/updates.mdx`.
