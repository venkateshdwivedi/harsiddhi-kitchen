# Lessons from earlier kitchen builds (Bhumi → Mangesh)

## Keep exactly as is (proven on a real phone)
- Header: `.top{position:sticky}`. Do NOT switch it to position:fixed.
- Call bar: position:fixed bottom + the visualViewport script that keeps it on the
  visible bottom edge. Do NOT remove that script.
- Do NOT add ScrollTrigger.config({ignoreMobileResize:true}).
These were "improved" once on Mangesh and broke on a real phone; reverting to the Bhumi
code fixed it. Browser-pane tests passed both times, so only a real phone shows this.

## Photos
- Use only photos uploaded by the business's own Google profile. In the Maps photo viewer,
  an owner upload shows a "View <business name>'s profile" link (a /maps/contrib/ link).
  A photo credited to a customer's name: skip it.
- The limited Maps view loads about 10 items. That's fine.
- Flag possible 3D renders (PNG, perfect lighting, nothing real through windows). If unsure,
  say so in DIRECTION.md and list it as a question for the client.
- Mid-install photos (protective film, tools on floor) are useful: caption them honestly.
- Export as .webp in img/ with explicit width/height. Portraits 900x1125, strip 700x875.

## Reviews & facts
- Quote short, exact lines from Google reviews; first name + initial.
- Anything not on the listing goes under "Labelled gaps": WhatsApp, Instagram, owner name,
  years in business, brands, warranty, prices, free site visit, showroom vs office.
- Don't put the Google rating into schema aggregateRating.

## Layout fixes already learned
- A hero photo pushes the quote form a full screen down on phones: hide it under 900px
  and show it further down the page instead.
- Focus outline must stay visible on dark sections too.
- 3D marble veins stay faint (alpha ≤ .4) or they look like cracks.
- At 320px the brand name must not wrap; shrink it.

## Borrow from Eat Move Rest (https://eat-move-rest-concept.netlify.app/)
- Tell the page as one project: small section labels like "Day 1 · Site visit",
  "Week 2–4 · Making & fitting", "Handover", "Years later" (only if a review supports it).
- A thin progress rail beside the 3D kitchen that fills through the build steps. It is part
  of the same scroll animation, not a second one.
- Flat colour blocks per section, taken from this client's own materials. No colour fades.
- One team card only if the client gives a real name and photo. At most one handwritten aside.

Do NOT borrow: scrolling marquees, breathing circle, drag carousel, loading screen.

## Must look different from earlier sites
- Bhumi: Fraunces + Instrument Sans; cream #F4EEE2, teal #123F3A, saffron #B5461B;
  plywood-edge motif; headline "Kitchens built to your walls, not a catalogue."
- Mangesh: Bricolage Grotesque + Figtree; marble #F1F0EC, taupe #4E443E, petrol #1D5870,
  amber #F3C975; LED-strip motif; headline "Bare walls in. A finished home out."

New site needs its own display + body fonts, five new hex values, its own static motif,
its own headline, and a finish set taken from its own photos.

## Checks before saying done
1. 1366px, 375px and 320px widths.
2. Scroll the whole page; tab through it; read the console.
3. Submit the form in preview mode.
4. No sideways scroll at any width.
5. Search for the previous client's details (name, phone, area, owner name).
6. Then test on a real phone over Wi-Fi.
