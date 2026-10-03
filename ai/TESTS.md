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

## TEST GAPs
- TEST GAP: no HTML validation / link check (would catch the missing `audio/*.mp3`).
