# Agent rules

- Tools and tasks live in `mise.toml`. Run `mise run check` before a change
  is done; CI runs the same task and `main` requires it.
- `mise run fix` applies the safe autofixes. `mise run links` checks external
  links (network, also weekly in CI).
- Do not disable a lint rule to get a change through. An exception is narrow
  (one element, rule or file), carries a reason, and needs a human decision.
- Pin GitHub Actions to a full commit SHA with the tag in a comment.
