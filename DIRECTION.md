# DIRECTION — Harsiddhi modular kitchen furniture (mockup)

Researched 24 Nov 2026 in the built-in browser, Google Maps place
`0x3bc2eb923799ffcd:0xdc1a9d8ea8b56a79` (limited Maps view).

## 1. References (one thing borrowed from each)

| URL | What we borrow |
|---|---|
| https://eat-move-rest-concept.netlify.app/ | The page told as one project: small sequence labels above sections, plus a thin progress rail beside the 3D kitchen that fills as the build steps advance. |
| https://www.reformcph.com/en | Fronts named as materials ("Sage matte", "Walnut"), not as colours, so the finish picker sounds like the person choosing the laminate. |
| https://www.vitsoe.com/ | Plain kit-of-parts rows: each thing they make gets one ruled row with the photo beside it. No cards. |

## 2. What this site feels like (one sentence)

A flat in Katraj on handover morning: sage and lilac shutters still smelling of laminate glue, a
walnut slat wall, and a phone number you can ring the same day.

## 3. Type and colour

- **Display:** Young Serif (Google Fonts, single weight 400)
- **Body:** Hanken Grotesk (400 / 600)
- **Devanagari name line:** Tiro Devanagari Hindi (the listing name is written in Hindi)

Five hex values, each taken from the business's own photos:

| Token | Hex | From |
|---|---|---|
| `--chalk` (page ground) | `#EDF0EA` | white panelled wall moulding, `wall-panel-fluted.webp`, warmed slightly towards the sage |
| `--sage` (flat section block) | `#CFDAD2` | sage wardrobe shutters, `wardrobe-sage.webp`, lightened for text contrast |
| `--walnut` (text + dark blocks) | `#2B1D16` | fluted walnut slats, `wall-panel-fluted.webp` (sampled `#3C251A`) |
| `--chevron` (calls to action) | `#8C3A45` | rose-maroon lower shutters cut in a chevron, `bedroom-chevron.webp` |
| `--navy` (reviews block) | `#233041` | velvet headboard, `bedroom-chevron.webp` (sampled `#2B303A`) |

Contrast targets: walnut on chalk ≈ 15:1, white on chevron ≈ 7:1, chalk on navy ≈ 12:1. All above AA.
I'll measure the real values in the browser at build time.

Different from earlier sites: no Fraunces, Instrument Sans, Bricolage or Figtree; none of
cream/teal/saffron or marble/taupe/petrol/amber; Mukta replaced.

## 4. Signature move + motif

**Signature move:** the page is cut like this client's own bedroom wardrobe. Each flat colour block
meets the next along a static two-peak chevron seam, the same shape as the rose-maroon shutters in
`bedroom-chevron.webp`. You can then repaint the 3D kitchen in the exact sage, lilac and walnut from
their photos.

**Motif (static, CSS clip-path):** the chevron seam at block edges, and on top of the quote form
(replacing Mangesh's LED strip). The motif never moves.

**Headline (draft):** "Measured once. Fitted room by room."
Different from Bhumi ("Kitchens built to your walls…") and Mangesh ("Bare walls in…").

**The one animated moment (unchanged mechanism):** while the build section is pinned, the 3D kitchen
assembles in five steps. The step list advances and a 3px progress rail beside the stage fills
(`scaleY`, from the same ScrollTrigger progress value). Nothing else on the page moves.
`prefers-reduced-motion` shows the finished kitchen and a full rail.

**3D finishes, from their own photos** (swatch hexes are set by eye; the photos are dim, so measured values are in brackets):

| Finish name | Hex | Photo |
|---|---|---|
| Sage matte | `#9DB0A6` (measured `#7F8787`) | `wardrobe-sage.webp` |
| Lilac gloss | `#8A5A88` (measured `#765162`) | `wardrobe-lilac.webp` |
| Walnut | `#5A3A28` grain (measured `#3C251A`) | `wall-panel-fluted.webp`, `bed-study-desk.webp` |
| Marble-white | `#E4DED6` with faint veins, alpha ≤ .4 (measured `#C9BEB3`) | white bands on `wardrobe-lilac.webp` |

Default finish: Sage matte. The oak plinth seen under the sage wardrobe (`#7C614B`) becomes the
plinth/kick colour in 3D.

**Project-sequence labels** (no durations, because the listing doesn't give any):
"Call · Site visit" → hero/form · "Making" → build section · "Fitting" → what we make ·
"Handover" → reviews. I'm leaving out "Years later" because no review supports it.

## 5. Facts from the listing

| Field | Value |
|---|---|
| Name on listing | **Harsddhi modular kitchen furniture.** (spelled with "dd", no "i", trailing full stop) |
| Hindi name on listing | **हरसिद्धि मॉड्यूलर किचन फर्नीचर.** (reads "Harsiddhi") |
| Category | Architect (as listed by Google) |
| Phone | 063773 44815 → `tel:+916377344815` |
| Address | Rajas Society, Katraj, Pune, Maharashtra 411046 |
| Plus code | FV38+53 Pune |
| Coordinates | 18.4529322, 73.865238 |
| Hours | **None listed** (the listing shows "Add hours") |
| Website | None listed |
| Rating | 5.0 from **1** review |
| Review tags | None |
| Attributes | LGBTQ+ friendly; wheelchair-accessible toilet |
| Maps link | https://www.google.com/maps/place/Harsddhi+modular+kitchen+furniture./@18.4529322,73.865238,17z/data=!4m6!3m5!1s0x3bc2eb923799ffcd:0xdc1a9d8ea8b56a79!8m2!3d18.4529322!4d73.865238!16s%2Fg%2F11z8tkhs7_ |

**Every visible review (1):**
- SwaropsinghSodha Sodha, edited about 5 months ago, 5★: "Safety doors and panling / Very very best 👌🔨"
  Owner replied: "Thank you so much". On the page: Swaropsingh S. The spelling "panling" is quoted as written.

**Owner / designer names:** none shown anywhere on the listing.

## 6. Photos (owner uploads only)

30 photos on the listing; the limited view loaded 10. 7 have the "View Harsddhi modular kitchen
furniture.'s profile" credit (owner uploads); 3 credited to SwaropsinghSodha Sodha were skipped.
All seven are phone photos (3000×4000, "Galaxy S26" watermark cropped out), with real views through
windows, bags and fans in frame. **None look like 3D renders.** All are dated **Jun 2026**.
All exported 900×1125 .webp.

| File | Source (Maps index) | What it shows | Render? |
|---|---|---|---|
| `img/wardrobe-lilac.webp` | #1, owner, Jun 2026 | Floor-to-ceiling hinged wardrobe, lilac high-gloss with white marble-look bands, long gold bar handles. **A worker stood in the original frame; cropped out.** | No |
| `img/bedroom-chevron.webp` | #2, owner | Bedroom: white wardrobe with rose-maroon chevron-cut lower panels, black/gold handles; walnut-sided storage bed with navy upholstered headboard | No |
| `img/wall-panel-fluted.webp` | #3, owner | White moulded wall panels between two fluted walnut slat strips, cove-lit false ceiling; a bag on the floor | No (mid-handover) |
| `img/wardrobe-sage.webp` | #5, owner | Sage matte wardrobe wall to the ceiling, round wooden knobs, oak plinth drawers | No |
| `img/niche-shelves.webp` | #6, owner | Wall niche with dark floating shelves and a fold-down wall table, window to a high-rise view | No |
| `img/living-panels.webp` | #8, owner | Living room: white moulded wall panels and a grey slatted strip. **Sofas, lamp and paintings may be bought furniture, not their work.** | No |
| `img/bed-study-desk.webp` | #9, owner | Small room: walnut-sided single bed with navy headboard and a built-in study desk with a marble-look top | No |

**There is no kitchen in any owner photo**, even though the business name says "modular kitchen".
The build section's 3D kitchen will be labelled "3D illustration, not a project photo", as on Mangesh.

## 7. How the photos map to the Mangesh structure

- Hero photo (desktop only, hidden under 900px): `wardrobe-sage.webp`
- Make 01 Modular kitchens: **no photo** (labelled gap); text points to the 3D build.
- Make 02 Wardrobes: `wardrobe-lilac.webp`, with `bedroom-chevron.webp` in the strip
- Make 03 Beds & study units: `bed-study-desk.webp`
- Make 04 Wall panelling & safety doors: `wall-panel-fluted.webp`, with a strip of `living-panels.webp` and `niche-shelves.webp`; on phones the strip also gets `wardrobe-sage.webp`, because the hero photo is hidden there
- Reviews block: one real quote (Swaropsingh S.), the 5.0 / 1 review shown plainly. I won't add invented reviews to fill the space.
- Visit block: "Rajas Society, Katraj." with **no hours line** (gap) and a "call before visiting" note.
- Schema: `HomeAndConstructionBusiness`, no `openingHours`, no `aggregateRating`.

## 8. Labelled gaps (ask the client)

1. **Spelling:** "Harsddhi" (listing) or "Harsiddhi" (Hindi name, folder)? The mockup uses
   **Harsiddhi** in display text and keeps "Harsddhi modular kitchen furniture." only where it must match Google.
2. **Kitchen photos:** none uploaded. Do they have any finished kitchens to show?
3. **Opening hours** and whether Rajas Society is a workshop, an office or a home address (can customers visit?).
4. **WhatsApp:** is 63773 44815 on WhatsApp?
5. **Owner / designer name and photo** (for the one team card, or skip it).
6. **Safety doors:** the one review praises them, but no photo shows a door. Do they have one?
7. **Living room photo:** did they make the sofas/lamp, or only the wall panels?
8. **Worker in the lilac wardrobe photo:** cropped out. OK, or do they want him shown with permission?
9. Brands of board/laminate/hardware, warranty, prices, free site visit, years in business,
   Instagram/Facebook. None of these are on the listing.
10. **Google category "Architect":** is that intended, or should it be "Kitchen furniture store"?
11. **Areas served** beyond Katraj (the form placeholder needs real nearby areas; I'll use
    Katraj, Dhankawadi, Ambegaon, Bibwewadi as placeholders until they confirm).
12. **Timings** for site visit → making → fitting. The sequence labels carry no durations until they confirm.
