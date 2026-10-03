# PROJECT — pose-demo-planemix50

> Derived from `README.md` ("Demo: QR produktside Alfix PlaneMix 50") and `index.html`.

## Purpose
Demo of a QR product page for the floor levelling compound Alfix PlaneMix 50 (20 kg bag): a mobile page reached from a QR code on the bag, with short step-by-step instructions and audio per step.

## User groups
- Craftsmen/DIY users scanning a QR code on the bag (assumed from README "QR produktside"; exact audience UNKNOWN / NEEDS CONFIRMATION).
- Prospective customer for the concept (manufacturer) — UNKNOWN / NEEDS CONFIRMATION.

## Main flows
1. Open page → "Brug til / Ikke til" → 5 steps (Underlag, Blanding, Påføring, Tørretid, Stop hvis), each with image placeholder, `<audio>` and short script.

## Core features
- Single static HTML file with inline CSS; no JavaScript; `noindex`.
- Audio sources `audio/01-underlag.mp3` … `audio/05-stop.mp3`.

## Integrations
None.

## Critical product rules (visible in code)
- Badge "Demo · ikke producent-godkendt" and footer "Ikke godkendt af Alfix", source alfix.com.
- Wet-room: membrane on top, never instead of it.

## UNKNOWN / NEEDS CONFIRMATION
- Hosting (GitHub Pages? Vercel?) — no config in repo. Public repository.
