# LUMIÈRE — Skin & Aesthetic Clinic — Design Package

Invented premium dermatology + aesthetics clinic. Promise: "Confidence, clinically delivered."
Voice: calm, medical-luxe, reassuring — spa feel, doctor's words. Footer discloses fiction + AI imagery.
Architecture: SOLÉA pipeline (scroll-scrub hero engine, cart→booking engine, lazy palindrome loops, mobile poster fallback). LIGHT site.

## Budget
Cap 250 credits (balance at start: 2,706.5 ✓). Stop and ask if projection crosses 230.

## The one call to action
Book a consultation → in-page booking widget → WhatsApp confirm (placeholder +910000000000) + in-page "Request received" state. Secondary: tel: "Call now". Trust line at every booking moment: "Free first consultation · Dermatologist-led · No-pressure plans."

## Customer language
Pain: "I've tried every cream", scars/pigmentation lowering confidence, fear of botched results, fear of pushy upselling.
Desire: natural-looking results, doctor-led not salon, transparent pricing, real before/afters.
Objections (FAQ): will it hurt · how many sessions · safe for Indian skin · pushy upselling.

## Palette (LIGHT)
--porcelain:#faf7f2 ground · --linen:#f0e9df panel · --ink:#1f2422 text · --sage:#8fa393 accent · --gold:#b99a5f rare accent (CTA/underline/glint)

## Type
Display: Cormorant Garamond (light). Body: Jost 300/400. Labels: Jost caps letterspaced. Prices/stats: tabular-nums.

## Signature elements
Gold thread SVG draws on scroll (SOLÉA technique, recolored) · Before/After clip-path drag sliders (no lib) · light-sweep on treatment cards hover · count-up stat counters (10,000+ sessions · 4.9★ · 12 yrs) · magnetic CTA · gentle input focus states.

## Hero film: "The Light Corridor" (6s 16:9 1080p Seedance)
Sun-washed minimalist clinic corridor, porcelain + pale wood, morning light through sheer curtains, slow dolly past sculptural reception desk with a single orchid, settles on treatment-room door opening onto soft light, gentle bloom, true rest. No faces close-up, no text, no logos. End frame = mobile poster + The Clinic image.
Start + end frames generated and reviewed BEFORE the film; film uses start_image + end_image.

## Beat map
1. 0–10% LUMIÈRE + "Skin & Aesthetic Clinic"
2. 16–30% "Confidence, clinically delivered."
3. 38–52% "Doctor-led. Results you can see."
4. 60–74% "Free first consultation."
5. 84–100% settle "Begin with a conversation." + CTA "Book your consultation"

## Treatments (6 cards: 1:1 start frame + motion loop, Kling 5s = cheapest proven)
| id | Name | Outcome line | Price | Loop still life |
|---|---|---|---|---|
| clear | Clear — Acne & scar revision | Smoother texture, fewer marks | from ₹2,500/session | serum droplet falling into glass dish, slow ripple |
| even | Even — Pigmentation & tone | Even tone, Indian-skin-safe lasers | from ₹3,500/session | laser handpiece resting on marble, soft light pulse |
| glass | Glass — HydraFacial ritual | The glass-skin glow | from ₹4,000/session | clear gel ribbon folding in slow motion, porcelain light |
| lift | Lift — Non-surgical contouring | Firmer lines, no surgery | from ₹8,000/session | rose-quartz roller on linen, light sweep |
| renew | Renew — Anti-aging | Softer lines, doctor-administered | ₹9,500 onwards | glass vial + orchid petal, slow gold glint |
| restore | Restore — Hair regrowth | Denser growth in 3 months | from ₹6,000/session | amber PRP vials in golden morning light |
Loop rules: slow elegant motion, warm porcelain light, nothing else moves, loop-friendly, no faces, no needles piercing skin, no gore, no text. Palindrome-encode for seamless loops.

## Before/After (3 pairs, 1:1, same synthetic face per pair via image-edit reference)
Acne-scar cheek · pigmentation jawline · under-eye. South-Asian skin tones, identical framing/lighting, subtle realistic improvement. Card label: "Simulated result — illustrative".

## Doctor portrait (1)
Confident Indian dermatologist, 40s, white coat, warm studio light, editorial. Marked "Illustrative". Credentials: Dr. Meera Kapoor, MBBS, MD (Dermatology) · 12 years. Quote: "My rule is simple. If it won't look natural, we don't do it."

## Sections
1 Hero journey → settle · 2 The Difference (Dermatologist-led / Transparent pricing / Natural results) · 3 Treatments (6 motion cards, "Add to consultation") · 4 Results (3 B/A sliders + stat counters) · 5 Your Doctor · 6 Reviews (5 cards, drag-scroll, 4.9★) · 7 Booking showpiece · 8 FAQ (accordion + FAQPage JSON-LD; MedicalClinic LocalBusiness schema, invented address) · 9 Footer (fiction + AI disclosure, hours, map placeholder).

## Booking widget (the showpiece)
Step 1 chips of selected treatments (empty = General consultation) → Step 2 14-day rolling date strip from today, skip Sundays + slot grid 11:00–19:30 30-min, ~30% "Booked" via deterministic per-date seed → Step 3 name + 10-digit phone (shake on error) → Confirm = WhatsApp prefill (treatments, date, slot, name) + in-page "Request received" state. Engine: SOLÉA cart engine, key = treatmentId, in-memory + localStorage.

## Performance/QA bar
Lighthouse ≥90 ×4 (screenshot to review/) · videos muted playsinline loop preload=none + poster, lazy IO; hero ≤3MB, loops ≤700KB · mobile poster cover + single column + horizontal date strip · reduced-motion kills scrub/loops · QA screenshots start/mid/end/mobile/booking to review/.

## SHOT LIST + credit math (estimates; actuals logged below)
| # | Asset | Model | Est |
|---|---|---|---|
| 1 | Hero start frame 16:9 2k | nano_banana_2 | 2 |
| 2 | Hero end frame 16:9 2k | nano_banana_2 | 2 |
| 3 | Hero film 6s 1080p | seedance_2_5 | 54 |
| 4–9 | 6 treatment stills 1:1 | nano_banana_2 | 12 |
| 10–15 | 6 loops 5s 1:1 | kling3_0 | ~48 (8 ea actual from SOLÉA) |
| 16–21 | 3 B/A pairs (before + edited after) | nano_banana_2 | ~14 |
| 22 | Doctor portrait 1:1 | nano_banana_2 | 2 |
| — | Re-roll headroom | — | ~15 |
| | **Projected** | | **~134–149 / 250** |

## Actuals log
- Batch 1 (12 stills): 24 cr
- After edits (3): 6 cr
- Hero start+end re-roll (signage tell + world continuity): 4 cr
- 6 Kling loops: ~48 cr (per SOLÉA actuals ~8 ea)
- Hero film Seedance: 54 cr
- Running: ~136 / 250 ✓ under the 230 tripwire

## QA results (2026-08-18)
- Lighthouse: Performance 99 · Accessibility 96 · Best Practices 96 · SEO 100 (report + screenshot in review/)
  - Fixes that got there: async Google Fonts (FCP 3.0s→1.0s), poster preload + fetchpriority, hero fetch deferred to load+idle
- Booking flow verified end to end: slot guard, 10-digit phone validation with shake, treatment chips, WhatsApp compose with date/slot/name, in-page confirmation state
- Date strip: starts today, Sundays skipped, ~30% seeded booked slots deterministic per date
- B/A sliders drag (pointer capture guarded), stat counters land on 10,000 / 4.9 / 12
- Reveal catch-up fix shipped: anchor landings (#booking etc.) render instantly
- Videos: hero 1.9MB (≤3MB), loops 100–300KB (≤700KB), palindromed seamless; posters everywhere; reduced-motion serves stills
- No horizontal overflow, both JSON-LD schemas present, fiction + AI disclosure in footer
- QA screenshots in review/: desktop top/treatments/results/booking/doctor, mobile top/treatments/booking, lighthouse
