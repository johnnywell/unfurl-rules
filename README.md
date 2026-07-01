# unfurl-rules

The open rule data behind [Unfurl](https://unfurl.software) — the on-device app that strips tracking parameters out of every link you copy or click.

Nothing here is hidden, and nothing is rebranded. Unfurl runs the open rule sets the privacy community already trusts, and adds its own small supplemental list to catch trackers the big lists miss. **Every rule Unfurl adds lives in this repo** — readable, auditable, and open to your pull requests.

## What's in here

| List | File | Format | License |
|------|------|--------|---------|
| Unfurl — supplemental clean-URLs | `rules/unfurl-clean.txt` | abp-removeparam | MPL-2.0 |
| Unfurl — supplemental debounce | `rules/unfurl-debounce.json` | brave-debounce | MPL-2.0 |

## The lists Unfurl builds on (fetched from their canonical sources, not bundled here)

| List | License | Source |
|------|---------|--------|
| ClearURLs | LGPL-3.0 | https://docs.clearurls.xyz |
| Brave clean-urls / debounce | MPL-2.0 | https://github.com/brave/adblock-lists |
| AdGuard URL Tracking | GPL-3.0 | https://github.com/AdguardTeam/AdguardFilters |

These keep their own names and licenses inside the app, exactly as their authors published them.

## How it's served

Unfurl fetches these over a CDN, cached:

```
https://cdn.jsdelivr.net/gh/johnnywell/unfurl-rules@main/rules/unfurl-clean.txt
```

Updating a rule here ships to every install **without an App Store review**.

## Found a tracker Unfurl misses?

Open a **Missed tracker** issue with the URL — that's half of why this repo is public. You don't need to know the rule syntax. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Unfurl's own rules (`rules/`) are **MPL-2.0** (see [LICENSE](LICENSE)). The upstream lists retain their own licenses.
