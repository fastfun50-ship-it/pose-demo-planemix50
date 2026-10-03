# STOP BEFORE MODIFYING THIS REPOSITORY.

Repository: `fastfun50-ship-it/pose-demo-planemix50` · Central standard: [SYSTEM117 AI Development Standard](https://github.com/fastfun50-ship-it/system117-ai-standard/blob/main/STANDARD.md)

1. Read `/ai/PROJECT.md`.
2. Read `/ai/RULES.md`.
3. Determine affected modules using `/ai/ARCHITECTURE.md`.
4. Read the relevant regression requirements in `/ai/TESTS.md`.
5. Inspect the actual implementation before changing anything.
6. Make the smallest possible change.
7. Run the required tests (`/ai/TESTS.md`).
8. If a regression occurs, the task is NOT complete.
9. Do not change architecture merely to solve a local problem.
10. Update status docs (`/ai/STATUS.md`) only where appropriate.

Before step 6, write the **EXPECTED CHANGE SCOPE** (files/modules, why, must-not-change, checks). If the real diff goes well outside it: stop and reassess.
Docs and code disagree? **STOP and report** — code is the truth of the implementation, `/ai` is the map.
**Critical User Flow Gate:** build/lint/typecheck/isolated tests green ≠ DONE. Name the affected critical user flows (`/ai/TESTS.md`). A change to a data chain or a function across modules needs at least one automated integration/E2E test proving the whole chain from input to visible result - otherwise the status is **TEST GAP** (state exactly what is not verified), never DONE.
**Data Contract Gate:** when data is produced/imported in one place and consumed in another, the test must verify that producer and consumer use the same schema/data source. No parallel hard-coded demo data may hide a broken integration. DONE report format: `/ai/RULES.md` §2c.

## Repo-specific hard stops
- The page is a **demo, not approved by the manufacturer** (badge + footer in `index.html`). Keep that disclaimer and the source attribution (alfix.com) visible.
- Product facts (mixing ratio, layer thickness, drying times, wet-room membrane warning) are abridged from Alfix' public text — do not invent or alter technical values without a source.
- `noindex` is set on purpose — do not remove it.
