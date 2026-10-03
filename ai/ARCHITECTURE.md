# ARCHITECTURE — pose-demo-planemix50

## Stack
One static file: `index.html` (HTML + inline `<style>`, no JS, no build, no package manager).

## Modules
| Module | Purpose | Main files | Depends on | May also affect |
|---|---|---|---|---|
| Page | Header/badge, use/not-use, 5 steps, footer | `index.html` | `audio/*.mp3` (not in repo) | everything |

No auth, API, DB, storage, admin, payments.

## Dependency map
| Change in | Regression-test |
|---|---|
| `index.html` | page renders on mobile (viewport-fit=cover), all 5 steps present, disclaimer + source visible, `noindex` kept |

## Deploy
UNKNOWN / NEEDS CONFIRMATION.
