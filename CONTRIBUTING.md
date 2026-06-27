# Contributing

Found a link Unfurl didn't fully clean? That's the most useful thing you can report.

## The easy way
Open a **"Missed tracker"** issue (the template prompts you for the URL and which parameters look like tracking). You don't need to know the rule syntax — just paste the link.

## Adding a rule directly
Rules live in `rules/`:
- `unfurl-clean-urls.json` — parameter stripping (Brave clean-urls format).
- `unfurl-debounce.json` — unwrapping redirect/wrapper links (Brave debounce format).

Keep additions tightly scoped and tested against a real example URL (include a before/after in your PR). Anything added here is also a good candidate to upstream to ClearURLs / Brave / AdGuard.

By contributing, you agree your additions are licensed under **MPL-2.0**.
