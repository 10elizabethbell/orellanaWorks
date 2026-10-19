---
name: Orellana Works LLC
description: The crew's own fall flyer made real, a forest-green yard the visitor rakes clear themselves.
colors:
  forest: "#173a26"
  forest-2: "#1f4a31"
  forest-3: "#26583a"
  lawn: "#4f8a39"
  lawn-top: "#5a9741"
  paper: "#eef3e7"
  paper-2: "#dfe8d4"
  rule-line: "#cad6bf"
  ink: "#17301f"
  ink-soft: "#44584a"
  cream: "#f6f0e1"
  cream-soft: "#d3e2c6"
  gold: "#e2a93b"
  gold-hover: "#efbd57"
  leaf: "#c8501e"
  lime: "#a6d96a"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.55rem, 11.2vw, 5.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.1rem, 9vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.375rem"
    fontWeight: 900
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.375rem"
    fontWeight: 800
    lineHeight: 1.3
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 800
    lineHeight: 1
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.55
rounded:
  field: "12px"
  card: "14px"
  lawn-corner: "36px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-phone: "20px"
  gutter-wide: "32px"
  max: "1120px"
  band-phone: "56px 0 64px"
  band-wide: "80px 0 92px"
  stack-sm: "10px"
  stack-md: "22px"
  stack-lg: "28px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.forest}"
    rounded: "{rounded.pill}"
    typography: "{typography.label}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-hover}"
    textColor: "{colors.forest}"
  service-row:
    textColor: "{colors.ink}"
    typography: "{typography.lead}"
    height: "58px"
  row-arrow:
    backgroundColor: "{colors.paper-2}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "40px"
  row-arrow-hover:
    backgroundColor: "{colors.leaf}"
    textColor: "#ffffff"
  link-card:
    backgroundColor: "{colors.forest}"
    textColor: "{colors.cream}"
    rounded: "{rounded.card}"
    padding: "18px 20px"
    height: "76px"
  step-badge:
    backgroundColor: "{colors.forest-3}"
    textColor: "{colors.gold}"
    rounded: "{rounded.circle}"
    size: "52px"
  chip:
    backgroundColor: "{colors.forest-2}"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.forest}"
  input:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "52px"
---

# Design System: Orellana Works LLC

## Overview

**Creative North Star: "The Fall Flyer, Made Real"**

The system is the crew's own autumn flyer turned into a yard you can touch. Forest green carries the ground of every dark band, a pale sage paper carries the light bands, cream and gold come straight off the logo's trim, and a rust-to-amber leaf palette lives only on the lawn. The page alternates dark forest and pale paper bands, and every seam between them is a living edge: rolling turf or swaying grass blades, never a straight rule.

Type is loud and plain. A system sans at 900 weight, uppercase and tightly set, does all the shouting; everything else is sentence-case, at a size meant to be read with one thumb on a phone. Density is low and the targets are big (44px minimum, 56px for the primary action). Ornament is limited to the lawn, the leaves and the grass; there are no photos, gradients-as-decoration or drop shadows on UI.

Interaction has one physical signature: a striped, mowed lawn under fallen maple, oak and elm leaves that a finger or mouse blows clear. Its motion is shared with the section edges through one animation loop that pauses anything offscreen and freezes to a still frame under reduced motion.

**Key Characteristics:**
- Forest / paper band alternation, joined by animated turf and grass edges.
- 900-weight uppercase system-sans display; plain sentence-case body at 17px.
- One gold pill call to action per view; lime is the interactive-state color on dark ground.
- The leaf lawn canvas is the signature component and the only place the autumn palette appears.
- Phone first: single column under 700px, the hero splits only at 1024px.
- Never black: the darkest values are greens.

## Colors

A logo-derived green, cream and gold palette with one rust action accent; the autumn reds and ambers belong to the leaves.

### Primary
- **Logo Forest** (forest): ground of the hero, the dark bands (How it works, Estimate), the Facebook link card, and the theme-color. Also the text color on gold.
- **Flyer Gold** (gold): the primary action fill, the focus ring everywhere, step numbers, the phone glyph, strong inline emphasis on dark ground, header/footer link hover. Hover lifts to **Warm Gold** (gold-hover).

### Secondary
- **Fresh Lime** (lime): the interactive-state color on forest ground. Input and chip hover borders, focus outlines on form fields, chips, the checkbox and the submit button; also the "WORKS LLC" wordmark line.
- **Raked Rust** (leaf): the hover/focus fill of the circular arrow on light paper rows. The one place a leaf color leaves the lawn, and only as a state.

### Tertiary
- **Mown Lawn** (lawn) and **Sunlit Turf** (lawn-top): the lawn's base and the top tone of its painted gradient; the grass edge that sits on each lawn uses lawn-top so the blades read as the same turf.

### Neutral
- **Sage Paper** (paper): page ground and light band background; never pure white.
- **Pale Sage** (paper-2): resting fill of row arrows on paper.
- **Field Line** (rule-line): 1px row dividers and the stroke line riding the turf edges on paper.
- **Deep Ink Green** (ink): body text on paper. **Moss Ink** (ink-soft): secondary text on paper.
- **Logo Cream** (cream): text on forest, input fields and the selected chip. **Sage Cream** (cream-soft): secondary text on forest.
- **Forest 2 / Forest 3** (forest-2, forest-3): footer ground, chip rest fill and the confirmation panel (forest-2); step badges, the card's arrow and the scrollbar thumb (forest-3).

### Named Rules
**The Never Black Rule.** No surface or text is black or neutral gray. The darkest value is ink (#17301f); shadows on the lawn are tinted green.

**The Leaves Stay On The Lawn Rule.** The eight autumn leaf colors live in the canvas CFG.COLORS array. In the UI, only Raked Rust appears, and only as the hover/focus state of an arrow.

**The Lime Means Live Rule.** On forest ground, lime is the hover and focus signal for every form control. Gold stays the fill of the action itself.

## Typography

**Display Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same stack

**Character:** One family, two voices. The flyer's heavy uppercase wordmark becomes the 900-weight display; the crew's casual, plain voice becomes sentence-case body. The system stack is a deliberate house choice: it is what the phones in Bound Brook already render, and it loads instantly inside Facebook's in-app browser.

### Hierarchy
- **Display** (900, clamp(2.55rem, 11.2vw, 5.6rem) on phone, clamp(3.2rem, 4.2vw, 4.75rem) at 1024px+, 0.95, uppercase, -0.02em, balanced): the hero slogan only, held to about 11ch on phone. The closing slogan uses a slightly larger headline (clamp(2.2rem, 9.5vw, 4.2rem), 12ch).
- **Headline** (900, clamp(2.1rem, 9vw, 3.6rem), 0.95, uppercase): section titles.
- **Title** (900, 22px / 1.375rem, 1.05, uppercase): service group names and step titles.
- **Lead** (800, 22px, 1.25 to 1.3, sentence case): service row labels, the Facebook card label, the service-area line. The hero promise uses the same 22px step at weight 400, line-height 1.45, max 34ch.
- **Body** (400, 17px / 1.0625rem, 1.55): default copy; prose capped at 44 to 46ch.
- **Label** (800, 17px, line-height 1): buttons, form labels, legends, the header phone number (tabular numerals).
- **Small** (14px / 0.875rem): the first-time-discount perk, form helper and error text, footer fine print.

### Named Rules
**The Three Body Steps Rule.** Running text uses only 14, 17 and 22px. Anything larger is uppercase 900 display.

**The Shout Once Rule.** Uppercase belongs to 900-weight headings and the logo wordmark. Body, labels, buttons and chips are sentence case.

## Layout

Phone-first, single column. Content sits in a centered wrap (max 1120px) with a 20px gutter that grows to 32px at 700px. Bands are padded 56px top / 64px bottom on phone and 80 / 92px from 700px. Vertical rhythm inside a band runs in roughly 10 / 22 / 28px steps (chip gaps, form field gaps, heading-to-content).

- **Under 700px:** everything stacks. The hero button is full width; the lawn fills the rest of the first viewport (min 250px) directly beneath the copy.
- **700px:** service groups go two-up, the work/area split becomes 1.1fr / 0.9fr, steps go three-up, the submit button returns to its natural width.
- **1024px:** the hero becomes a two-column grid (1.15fr copy / 0.85fr lawn) with the header spanning both; the lawn gets a 36px top-left corner and the grass edge above it is hidden. Name and town fields pair up; the form widens to 760px.

Breakpoints are min-width only. The lawn's own phone/desk split (leaf size, blower radius) keys off max-width 699px so it agrees with the CSS.

## Elevation & Depth

The UI is flat. There are no box-shadows on any component; depth comes from tonal banding (forest against paper, forest-2 and forest-3 inside forest) and from the edges overlapping the band above by 45px. The only shadows in the system are on the lawn canvas, where each airborne leaf casts a green-tinted shadow (rgba(20,40,16,.42)) offset by its height.

### Named Rules
**The Flat UI, Deep Lawn Rule.** Shadows are physics, not chrome. They exist only under leaves in the air.

## Shapes

Soft and round, with no sharp corners on interactive surfaces. Actions and chips are full pills (999px); every icon disc, arrow and step badge is a circle; the link card is gently rounded (14px), fields slightly less (12px). The one large curve is the hero lawn's 36px top-left corner at desktop width. Section boundaries are never straight lines: they are the turf and grass edges below.

### Section edges
Each band boundary is a 46px-tall SVG, full width, pulled up 45px over the previous band, redrawn per frame to its own pixel width.
- **Turf** (onto paper or the footer): a rolling ground line from three summed sines (speed 1.1), filled with the next band's color, with a 2.5px rule-line stroke riding 5px above it.
- **Grass** (onto forest, and on top of each lawn): individual blades every 7px, each with its own height (14 to ~41px) and lean, swaying at speed 1.6.
Turf leads into light bands, grass into dark bands and lawns.

## Components

### Buttons
Big, warm and unmistakable.
- **Shape:** full pill (999px), 56px tall, 2px border matching the fill.
- **Primary:** gold fill, forest text, 800-weight 17px label, 26px side padding (34px on the wide form). Full width on phone in the hero and the form.
- **Hover / Focus:** fill lifts to warm gold; press nudges 1px down (disabled under reduced motion). Focus is the global 3px gold ring offset 3px; on the forest form, hover and focus add a 2px lime outline.
- There is one button style. Secondary actions are text links (800 weight, underlined, padded to a 44px hit area).

### Chips
- **Style:** pill, 46px tall, forest-2 fill, 2px #3d6b4c border, cream 700-weight text. Real checkboxes, visually hidden.
- **State:** hover and keyboard focus turn the border lime (focus adds a 2px lime outline); checked inverts to a cream fill with forest text.

### Cards / Containers
- **Corner Style:** 14px.
- **Background:** forest on paper.
- **Shadow Strategy:** none (see Elevation).
- **Internal Padding:** 18px 20px, min 76px tall.
- The Facebook link card is the one card: brand-blue icon disc left, 22px lead label, forest-3 arrow disc pushed right that turns gold on hover.

### Inputs / Fields
- **Style:** cream fill, ink text, 2px transparent border, 12px radius, 14px 16px padding, min 52px (textarea 110px, vertical resize). Placeholder #5a685c.
- **Focus:** hover turns the border lime; focus adds a 2px lime outline offset 2px.
- **Error:** border #ff9b7a with a 14px #ffc9b5 message beneath, shown only after a submit attempt. The confirmation is a forest-2 panel with 12px radius.
- **Checkbox:** native, 24px, gold accent, lime outline on hover/focus.

### Navigation
- **Header:** logo mark plus stacked wordmark ("ORELLANA" 900, "WORKS LLC" lime, tracked) on the left; the tap-to-call number top-right in cream 800 tabular numerals with a gold phone glyph, gold on hover. Not sticky.
- **Footer:** forest-2 ground, phone and Facebook as 44px-tall cream links that turn gold on hover.

### Service Rows
A list of full-width links, 58px tall, 22px 800-weight ink labels between 1px rule-line dividers. The only hover cue is the 40px circular arrow on the right: pale sage at rest, rust fill with white glyph on hover and focus (focus adds a 3px rust ring). The row itself never changes background or gains a shadow. Each row pre-checks its matching chip in the estimate form.

### Step List
Numbered by CSS counter: a 52px forest-3 disc with a 900-weight gold numeral, a 22px uppercase title beside it, sage-cream body below (max 44ch). Stacks on phone, three-up from 700px.

### Leaf Lawn (signature)
A canvas of a striped, mowed lawn (gradient lawn-top to #3e732f, faint diagonal stripes, ~9000 hand-scattered blades) under overlapping maple, oak and elm leaf sprites in eight autumn colors. Pointer movement blows leaves out of a radius; they lift, tumble with a cast shadow and drift back in. Used twice: the hero (vertical drag captured) and the close (page scroll allowed, touch-action pan-y).

Tunables live in the CFG object and are the system's knobs: leaf size 16px phone / 22px desk, coverage 2.6, max 3400 leaves, blower radius 62 / 88px, force 2300, carry 0.9, lift 260, gravity 520, ground/air drag 7.5 / 0.9, refill 12 leaves/s, fall speed 46, gusts every 5 to 9s, autoplay after 5s idle, DPR capped at 1.5.

**Motion rules.** One shared requestAnimationFrame loop drives both lawns and every section edge; dt is clamped to 1/240 to 1/30s. Each lawn and edge pauses when offscreen (IntersectionObserver). Under prefers-reduced-motion, lawns and edges paint one still frame, the loop never starts, the hint line is hidden, smooth scroll and press nudges are off. Untouched for 5s, the hero lawn sweeps itself so it reads as alive on first view.

## Do's and Don'ts

### Do:
- **Do** alternate forest and paper bands and join every pair with a turf edge (into paper) or grass edge (into forest or a lawn), pulled up 45px.
- **Do** set every heading in the system sans at 900, uppercase, -0.02em, line-height 0.95.
- **Do** keep running text to 14, 17 and 22px, sentence case.
- **Do** use the gold pill (56px, forest text) for the one primary action in a view.
- **Do** use lime for hover and focus on forest-ground controls, and the 3px gold ring for focus elsewhere.
- **Do** give every tap target at least 44px.
- **Do** run any new animation off the shared loop, pause it offscreen, and give it a reduced-motion still frame.
- **Do** tune the lawn through CFG rather than editing the physics.

### Don't:
- **Don't** use black or neutral gray anywhere; the darkest value is ink green.
- **Don't** put drop shadows on UI components; shadows exist only under airborne leaves.
- **Don't** use the autumn leaf colors as UI colors; rust is only the row-arrow state.
- **Don't** use a straight rule or hard edge between bands.
- **Don't** add hover backgrounds or shadows to service rows; the arrow is the cue.
- **Don't** start a second requestAnimationFrame loop.
- **Don't** add a sticky header or bottom call bar; the phone number lives top-right on the first screen.
