# RULES — pose-demo-planemix50

Fælles indgang: [README](https://github.com/fastfun50-ship-it/system117-ai-standard/blob/main/README.md). Eneste fælles regelkilde: [STANDARD.md](https://github.com/fastfun50-ship-it/system117-ai-standard/blob/main/STANDARD.md). Kopier af fælles roller, gates, scope og DONE-format er fjernet herfra. Slå de relevante afsnit op i kilden; nedenstående særkrav og godkendte projektundtagelser bevares.

## 3. Repo-specific rules (evidenced in `index.html`)
- Keep the "ikke producent-godkendt" disclaimer, the source line and `noindex`.
- Technical product values only from the manufacturer's public text.
- Keep it a single static file — adding a framework/build = ARCHITECTURE DECISION.

## 4. Deploy / branches
- **One development line (default, STANDARD.md §9a):** one active development line → one version we test → one deployment we keep building on. Do not spread an ordinary task over several branches/environments on your own. Preview/staging only when this repo has real customers/data or Peter asks - and then it is written here as a project override.
- Default branch `main`. Repository is **public**. Deploy: UNKNOWN / NEEDS CONFIRMATION.

## 5. ARCHITECTURE/PRODUCT DECISION REQUIRED
- Removing the demo disclaimer / presenting as official manufacturer page.
- Adding tracking/analytics.
