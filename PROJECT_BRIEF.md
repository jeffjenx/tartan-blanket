# Tartan Blanket — Project Brief

**Status:** Prototype 05 built and reviewed. Pre-production — no supplier, no sample, no checkout.
**Source of truth:** `github.com/jeffjenx/tartan-blanket` (this file lives in the repo root).
**Goal:** First original manufactured product under the LLC. A real release, not a prototype.

## The product

Custom reversible blankets under the brand **Jeff Jenx Blankets & Textiles** (Collection Vol. 01 — "Comfort, with character"). Customers pick a signature colorway or design their own plaid (colors, structure, dimensions, materials, border) in the on-page designer, then buy ready-made, request made-to-order, or get DIY instructions. The site itself is the storefront and the configurator.

## What's built (Prototype 05)

- Single-file site (`index.html`, no dependencies): hero, 5-colorway collection, 40+ swatch colorway archive, 6-step blanket designer with live canvas preview, DIY/maker section.
- 5 signature colorways with final hex palettes: Nocturne, Meridian, Wisteria Vale, Winterbourne, Emberwood.
- "Save design brief" exports a `.txt` spec sheet — the intended manufacturing handoff format.
- Careful "inspired by, not licensed" disclaimers on sports/console/world palettes. Keep this posture.

## Decisions locked

| Decision | Date |
|---|---|
| Brand: Jeff Jenx Blankets & Textiles, Vol. 01 | Proto 05 (Oct 2026) |
| 5 signature colorways + hex palettes (see code `presets`) | Proto 05 |
| 5 plaid structures: heritage, windowpane, buffalo, pinstripe, asymmetric | Proto 05 |
| Reversible construction; signature frame border 0–6 in | Proto 05 |
| 3 fulfillment paths: ready-made / made-to-order / DIY | Proto 05 |
| Size presets throw 50×60 → Cal King 108×96, custom allowed | Proto 05 |
| Material shortlist (front/reverse/middle) | Proto 05 |
| Reference spec: 70 × 90 in (personal example) | Proto 05 |

## Open questions (in dependency order)

1. **Woven vs printed?** The single biggest fork. Custom woven tartan = high MOQs, premium feel. Printed = low MOQ, full custom colorways, faster. Gates supplier search and pricing.
2. **Launch lineup:** Nocturne-only to start, or all five colorways?
3. **Target retail price + margin.** Set before talking to suppliers, not after.
4. **Supplier:** domestic vs overseas; cut-and-sew vs full-package.
5. **Sales channel:** this site + checkout (Stripe/Shopify?) vs Etsy vs both.
6. **DIY path:** real product or marketing? Decide — it has a full section.
7. **Legal:** FTC textile labeling (fiber content, care, origin); "Jeff Jenx" trademark.

## Next 3 actions

1. Make the woven-vs-printed call.
2. Set target price and margin → gives suppliers a cost target.
3. Get quotes from 3 suppliers against the Nocturne 70×90 reference spec.

## Definition of done

Physical sample approved in hand → landed unit cost at/under target → first batch listed for sale under the LLC and shippable. Prototype → sample → launch is a pipeline with exits, not a loop.

## Phase plan

- **Phase 0 — Design freeze.** Lock the launch spec (colorway, dimensions, materials, construction). *Gate: brief v1.0 committed.*
- **Phase 1 — Sourcing.** Woven/printed decision, 3+ quotes, MOQ + landed cost + lead time. *Gate: supplier selected, margin confirmed.*
- **Phase 2 — Sample.** Physical sample ordered; wash/wear test; color check vs the canvas preview. *Gate: sample approved in hand.*
- **Phase 3 — Storefront.** Prototype → real site: optimize assets, add checkout, packaging, care labels. *Gate: end-to-end test order completes.*
- **Phase 4 — Launch.** First small production run, list, fulfill. *Gate: first batch shipped.*
- **Phase 5 — Iterate.** Made-to-order path, DIY product, more colorways.

## Watch-outs

- **Asset weight:** the 5 hero PNGs total ~18 MB. Must be optimized (resize/compress, modern formats) before any real launch — Phase 3 task.
- **Preview ≠ fabric:** the canvas preview communicates layout/color only. Already disclaimed in the UI; keep managing that expectation through sampling.
- **Licensing:** the "inspired by" palette strategy works only with the current explicit disclaimers. Never imply endorsement.
- **No commerce yet:** no checkout, no order pipeline, no quote integration — all Phase 3+.

## Working agreement

This repo is the shared brain. AI assistants work via MCP against this repo; changes arrive as diffs/commits for human review before merge. Briefs and decisions live here, not in chat windows.
