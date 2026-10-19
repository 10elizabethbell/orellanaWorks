# Orellana Works LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/orellanaWorks/ · **Repo:** https://github.com/10elizabethbell/orellanaWorks · **Built:** 2026-10-18 from Muse brief (run 2026-10-18, NJ Small Business Network group post)

## What's built
- One page, `index.html` (~45KB, no images embedded, system fonts, no tracking). Phone layout first; desktop splits the hero into copy left / lawn right at 1024px+.
- **World: fall lawn.** Their logo's forest green and cream with gold trim, plus the flyer's autumn leaf colors. The ground is never black.
- **Signature element:** a striped, mowed lawn under a blanket of maple, oak and elm leaves (`#lawn-hero`). A finger or mouse works as a leaf blower: leaves get pushed, carried along, lifted and flipped, then blown off the edge, and they drift back down over the next few seconds. It sweeps itself on autoplay until touched, gusts skitter the top layer now and then, and the hint fades after the first touch. On phones you can drag up, down and sideways (it reads the canvas position every frame and turns off pull-to-refresh). The same lawn returns above the footer (`#lawn-close`, `pan-y` so the page still scrolls there).
- Section edges: rolling turf lines (green to light) and swaying grass blades (light to green), all on one shared animation loop that pauses off screen. Reduced motion gets a still frame.
- Sections: header (logo mark redrawn from their flyer, tap-to-call number top right) → hero (their slogan "Your property, our priority.", one gold "Get a free estimate" button, first-time discount line) → What we do (Yard / Build rows; each row ticks that service in the form) → How it works (3 steps) → See our work (big Facebook card) + Where we work → Free estimate form → "Quality work, affordable prices." (their tagline) on a light band over the second lawn → footer (name, phone, Facebook). Grass blades fringe the top of each lawn on phones.
- **Contact:** the form checks the fields, then opens a pre-filled text to +1 908-356-2628 (name, services, town, details, and a "first time hiring you, is there a first-time discount?" line if ticked). A call link sits right under the button.
- `og.jpg` (1200×630 hero shot) for the Facebook preview; favicon (SVG) and `apple-touch-icon.png` use the roof-and-leaf mark.

## Assumptions I made
- **Crew voice ("we"):** LLC, truck and trailer on the flyer, "Your property, our priority."
- **Logo mark:** redrawn as SVG from the flyer logo (roof with a window, pines, swoosh, leaf). It's not their file. The Facebook profile image (white "ORELLANA / WORKS" on black with gold rules) had a "new page" badge over it, so I didn't use it.
- **Grouping services as "Yard" and "Build":** my grouping. "Remodeling & construction" is merged into one row. "And much more" became "Something else on your property? Ask us."
- **How-it-works copy** ("straight price before any work starts", "the way we'd want it done at our own house"): inferred from "FREE ESTIMATES" and "Quality Work". The owner should confirm.
- **Texting:** the brief says texts are unknown. The form hands off by text with a call fallback right below it. If 908-356-2628 is a landline, switch the form to call-only.

## Placeholders and gaps
- **No real work photos.** The flyer's photos (truck, deck, driveway, leaf blower) look AI-generated, so I didn't present them as their jobs. "See our work" is just the Facebook link for now. Real photos (ideally before/after pairs) are the biggest upgrade.
- No email (so none in the footer), hours, owner name, reviews, prices, years in business or street address. None of these appear on the page.
- The Facebook card says "See our work on Facebook." rather than your usual "Click to see more of my work.", because no work photos sit above it. Muse couldn't read their page, so check it actually shows job photos; if it doesn't, change the card to "Follow us on Facebook."
- The Facebook URL is the `profile.php?id=` form. A vanity URL would look nicer if they have one.

## Questions for the owner
- Does 908-356-2628 take texts?
- Can you send photos of real jobs, especially before/after (cleanups, patios, concrete, decks)?
- An email for the footer? Hours? Your first name ("Ask for ___")?
- Which towns around Bound Brook do you cover?
- What is the first-time discount (amount or %)?
- Which services matter most to you? Fall cleanups lead right now; that should change with the season.

## Ideas not built (yours to pick)
- **Runner-up world:** fresh concrete. The hero is a wet gray slab you trowel smooth with your finger, with broom-finish texture and edging lines. It suits their construction and concrete side better; the lawn suits the season.
- Seasonal swap: in spring, the lawn could be mowed by the finger (stripes appear) instead of leaf-blown, and snow removal in winter if they offer it.
- A few leaves flutter off a service chip when it's ticked (like Sunny Side's splash).
- When the form is submitted, blow the closing lawn clear ("request sent = yard cleared").
- A photo strip, framed as leaves landing on the lawn, once real photos exist; before/after sliders with a plain gold divider.
- A licensed display face to match the flyer's heavy wordmark (house style kept the system stack).
- A Spanish toggle, if the owner wants to reach Spanish-speaking customers (owner preference unknown).

## Not verified
- Real-device touch (tested with synthetic touch in Playwright Chromium and WebKit at 360/390/430px wide).
- The real SMS handoff on iOS and Android (body encoding verified; `?&body=` on iOS, `?body=` on Android).
- Frame rate on older phones (~1,000 leaves on a 390px phone, up to 3,400 on desktop; tune `CFG` at the top of the lawn script).
- How the page looks inside Facebook's in-app browser itself.
