<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Español](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Castile and León only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-26 06:22 UTC, BOE consolidated legislation, autonomous communities (open data): 25 addresses read; 0 added, 0 changed, 0 removed; no change; 2 not published, 0 of them with no reason. Flags: `publish-lag`, `audit-disagrees`.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [BOE consolidated legislation, autonomous communities (open data)](https://www.boe.es/datosabiertos/api/api.php) | `estatuto-de-autonomia/`, `ley-*/`, `decreto-ley-*/`, `decreto-legislativo-*/`, `…` | daily | 2026-11-26 06:22 UTC | no change | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-26 06:22](checks/2026-11.md#es-boe-autonomico-20261126t062215z) | boe-autonomico | 25 | 0 | 0 | 0 | 2 (0) | no change `publish-lag` `audit-disagrees` | — |
| [2026-11-25 06:17](checks/2026-11.md#es-boe-autonomico-20261125t061751z) | boe-autonomico | 25 | 0 | 0 | 0 | 2 (0) | no change `publish-lag` | — |
| [2026-11-24 07:17](checks/2026-11.md#es-boe-autonomico-20261124t071754z) | boe-autonomico | 25 | 0 | 0 | 0 | 2 (0) | no change `publish-lag` | — |
| [2026-11-23 13:52](checks/2026-11.md#es-boe-autonomico-20261123t135251z) | boe-autonomico | 24 | 0 | 0 | 0 | 2 (0) | no change `audit-disagrees` | — |
| [2026-11-23 01:08](checks/2026-11.md#es-boe-autonomico-20261123t010811z) | boe-autonomico | 10 | 0 | 0 | 0 | 2 (0) | no change | — |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
