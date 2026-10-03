# TESTS — pose-demo-planemix50

## Existing automated checks
None (no package.json, no build). BUILD: n/a (static file).

## CI
None. No `ai-gate.yml` added — there are no existing commands to run.

## Critical manual flows
1. Open `index.html` on a phone: header, badge, both use cards, 5 steps, footer.
2. Each `<audio>` plays its MP3 (currently files missing — see STATUS).

## Regression matrix
| Area changed | Must re-verify |
|---|---|
| `index.html` | flows 1–2 |

## Critical user flows (Critical User Flow Gate / Data Contract Gate)

- The numbered list under "Critical manual flows" is this repo's **critical user flow list** (STANDARD.md §2a). Name the affected flows by number in every DONE report (`/ai/RULES.md` §2c).
- A flow is only proven when an automated integration/E2E test covers the whole chain from input to visible result. A cross-module change touching a flow without such a test is reported as **TEST GAP**, never DONE.
- Data Contract Gate: producer and consumer of shared data must be tested against the same schema/data source; hard-coded demo data must not mask a broken integration.
- Data Source Gate: tests use the real source (or a clearly marked fixture copied from it) and must fail loudly when the source is missing/broken; synthetic data must never replace required real base data to reach a count or turn a check green.

## TEST GAPs
- TEST GAP: no HTML validation / link check (would catch the missing `audio/*.mp3`).
