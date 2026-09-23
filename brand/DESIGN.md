# Chilli Community design system

A chilli-only digital membership that helps beginners grow chillies, cook simple recipes, watch recipe demonstrations and share what they make.

**Why this look:** it is calm, warm and plain, with real windowsill photos and one orange, so someone who gave up after one dead plant feels welcome, not talked down to by experts or a cartoon. In Priya's words: it feels like a club, not a shop.

The CoEngineers design system, with one change. Every CoEngineers token in this file (colours, spacing, radius, components) matches the CoEngineers house style value for value, because the Chilli case study and videos are already built on it. The one change: small uppercase labels are set in Inter, so Chilli uses two typefaces, not three. Chilli's own parts are the wordmark, the mark, two extra colours for small details, the imagery rule and the voice.

- Status: Decided. Priya, 23 September 2026: "Coengineers exactly as we've already done the case study and base videos." Priya, 30 September 2026 (Week 4): kept the colours, the two extra colours (leaf and chilli), the voice rules and the one accent as drafted, and chose two typefaces, with small labels in Inter
- Last changed: 30 September 2026
- Brand kit: `brand/brand-kit.html`
- Logo files: `brand/logo-wordmark.svg`, `brand/logo-mark.svg`, with PNG copies (`.png`) for tools that cannot take SVG

Every skill reads this file and uses the tokens below by name. Spacing, type scale and radius are the same in every CoEngineers variant, so templates can rely on them.

## Feel

Warm editorial, the CoEngineers feel: calm, premium, content first. A warm paper page, near-black ink, generous space and one orange for the thing that matters. For Chilli that means real windowsill and kitchen photos on that paper, and words a beginner grower can act on this week. Three words: warm, homegrown, calm. Friendly, never childish (Decided, Priya, 30 September 2026). It is for beginner growers on a windowsill, a balcony, in a garden or in a greenhouse.

## Colour

| Token | Value | Role |
|---|---|---|
| `colour.canvas` | `#FBFAF8` | Page background |
| `colour.surface` | `#FFFFFF` | Cards, photo and illustration stages |
| `colour.recessed` | `#F2EFE8` | Side panels, quiet bands, table headers |
| `colour.ink` | `#232421` | Body and heading text |
| `colour.muted` | `#696961` | Secondary text, captions, metadata |
| `colour.primary` | `#F7931A` | The one accent: the main button, one job |
| `colour.on-primary` | `#101014` | Text and icons on `colour.primary` |
| `colour.hairline` | `#E9E7E1` | Quiet separators (decorative only) |
| `colour.focus` | `#A35809` | Focus ring, 3px with a 3px offset |
| `colour.band` | `#1A1A1A` | Rare dark statement band, `colour.canvas` text on it |
| `colour.secondary` | `#232421` | No second brand colour: quiet actions and link underlines use ink |
| `colour.on-secondary` | `#FBFAF8` | Text on `colour.secondary` |
| `colour.primary-soft` | `#FDE9CC` | Tint behind a highlighted chip or note, ink text on it |
| `colour.secondary-soft` | `#F2EFE8` | Tint behind a "Decided" chip or a tip, ink text on it |
| `colour.field-border` | `#8C877C` | Form field and checkbox borders (3:1 or more) |

`colour.primary` as text: never. Orange is 2.2:1 on canvas, so it is for fills only: the main button. The one exception is the wordmark, where "Chilli" is set in orange as a logo, the same as "Co" in the CoEngineers wordmark. Logos are exempt from the text contrast rule, and "Community" in ink carries the name.

The accent is restrained: never a broad wash, never decoration, never status on its own. Its one job is to mark the single main button on a page (Decided, Priya, 30 September 2026). The orange "Chilli" in the wordmark is part of the logo and is not counted.

### Extras

Chilli's own extras sit on top of the CoEngineers tokens. They never replace one, and they are for small details only. Status: Decided (Priya, 30 September 2026, kept as drafted).

| Token | Value | Use | Lowest check |
|---|---|---|---|
| `colour.leaf` | `#3D6A2B` | A small growing detail: a "Growing" tag, a plant label, the leaf in a drawing | 5.5:1 on `colour.recessed` |
| `colour.chilli` | `#B3301E` | A small cooking detail: a "Recipe" or heat tag, the pod in a drawing | 5.4:1 on `colour.recessed` |

- As text or a 1px outline on `colour.canvas`, `colour.surface` or `colour.recessed` only. Never a fill behind text, never the main action, never a status on its own.
- One extra per detail, and the word always carries the meaning. Never put leaf and chilli side by side as blocks: some readers cannot tell red from green.
- Never next to the orange button as a competing colour. The page still has one accent, and it is orange.

### Checked pairs (WCAG AA)

Normal text needs 4.5:1. Large text (24px and up, or 19px bold) and field borders and focus rings need 3:1. Re-measured by code on 30 September 2026; every value below matches.

| Pair | Ratio | Used for | Result |
|---|---|---|---|
| `colour.ink` on `colour.canvas` | 14.9:1 | Body text on the page | Passes AA |
| `colour.ink` on `colour.surface` | 15.6:1 | Text on cards | Passes AA |
| `colour.ink` on `colour.recessed` | 13.5:1 | Text on quiet panels | Passes AA |
| `colour.muted` on `colour.canvas` | 5.3:1 | Captions and details | Passes AA |
| `colour.muted` on `colour.surface` | 5.5:1 | Captions on cards | Passes AA |
| `colour.muted` on `colour.recessed` | 4.8:1 | Captions on quiet panels | Passes AA |
| `colour.primary` on `colour.canvas` | 2.2:1 | Accent as text | Fills only, never text |
| `colour.primary` on `colour.surface` | 2.2:1 | Accent as text on cards | Fills only, never text |
| `colour.primary` on `colour.recessed` | 2.0:1 | Accent as text on quiet panels | Fills only, never text |
| `colour.secondary` on `colour.canvas` | 14.9:1 | Quiet actions (ink) | Passes AA |
| `colour.secondary` on `colour.surface` | 15.6:1 | Quiet actions on cards | Passes AA |
| `colour.secondary` on `colour.recessed` | 13.5:1 | Quiet actions on quiet panels | Passes AA |
| `colour.on-primary` on `colour.primary` | 8.2:1 | Primary button label | Passes AA |
| `colour.on-secondary` on `colour.secondary` | 14.9:1 | Text on the secondary colour | Passes AA |
| `colour.ink` on `colour.primary-soft` | 13.1:1 | Testing chip, highlighted note | Passes AA |
| `colour.ink` on `colour.secondary-soft` | 13.5:1 | Decided chip, tip | Passes AA |
| `colour.canvas` on `colour.band` | 16.6:1 | Statement band | Passes AA |
| `colour.primary` on `colour.band` | 7.5:1 | "Chilli" in the wordmark on the band | Passes (3:1 for large text) |
| `colour.field-border` on `colour.canvas` | 3.4:1 | Form field edge on the page | Passes (3:1 for edges) |
| `colour.field-border` on `colour.surface` | 3.5:1 | Form field edge on cards | Passes (3:1 for edges) |
| `colour.focus` on `colour.canvas` | 5.0:1 | Focus ring on the page | Passes (3:1 for edges) |
| `colour.focus` on `colour.surface` | 5.3:1 | Focus ring on cards | Passes (3:1 for edges) |
| `colour.leaf` on `colour.canvas` | 6.1:1 | Growing tag on the page | Passes AA |
| `colour.leaf` on `colour.surface` | 6.3:1 | Growing tag on cards | Passes AA |
| `colour.leaf` on `colour.recessed` | 5.5:1 | Growing tag on quiet panels | Passes AA |
| `colour.chilli` on `colour.canvas` | 5.9:1 | Recipe tag on the page | Passes AA |
| `colour.chilli` on `colour.surface` | 6.2:1 | Recipe tag on cards | Passes AA |
| `colour.chilli` on `colour.recessed` | 5.4:1 | Recipe tag on quiet panels | Passes AA |

## Type

Two typefaces only.

| Token | Value | Weights and use |
|---|---|---|
| `font.display` | `Space Grotesk` | 500 and 600. Headings, the wordmark, big numbers |
| `font.body` | `Inter` | 400, 500 and 600. Body, controls, small uppercase labels |
| `font.stylesheet` | `https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600&family=Inter:wght@400;500;600&display=swap` | The Google Fonts link that loads both. A template that says `font.import`, `font.link` or `font.url` means this link |

There is no third face. A template that asks for `font.mono` uses `font.body` instead.

Type scale (the same in every CoEngineers variant):

| Token | Size and line height | Face |
|---|---|---|
| `type.page` | 34 to 46px (fluid), 1.12 | `font.display` |
| `type.section` | 23 to 26px, 1.25 | `font.display` |
| `type.card` | 20px, 1.3 | `font.display` |
| `type.lead` | 19px, 1.55 | `font.body` |
| `type.body` | 16 to 18px, 1.65 | `font.body` |
| `type.small` | 14px, 1.5 | `font.body` |
| `type.label` | 12px, uppercase, letter spacing 0.06em | `font.body` (Inter 500) |

Sentence case for every heading. Reading width 65 to 75 characters.

## Spacing and radius

| Token | Value |
|---|---|
| `space.1` | 8px |
| `space.2` | 12px |
| `space.3` | 16px |
| `space.4` | 24px |
| `space.5` | 32px |
| `space.6` | 48px |
| `space.7` | 64px |
| `radius.card` | 18px |
| `radius.image` | 12px |
| `radius.button` | 9px (form fields too) |
| `radius.pill` | 999px (chips, progress tracks, avatars) |

Card padding `space.4` to `space.5`. Between major sections `space.5` to `space.6`. Fewer boxes: use headings and space before borders. Shadows, if any, barely visible.

## Components

- **Primary button:** `colour.primary` fill, `colour.on-primary` text, `font.body` 600, at least 44px tall, `radius.button`. One per view: the one thing the reader should do.
- **Quiet button:** no fill, `colour.ink` text, 1px `colour.hairline` border, `radius.button`.
- **Card:** `colour.surface`, `radius.card`, padding `space.4`. Only for things that are genuinely separate; most reading sits on `colour.canvas`.
- **Chip:** `radius.pill`, 12px `font.body` 600, optional dot. Status chips always carry the word: **Decided** (`colour.secondary-soft`, filled dot), **Testing** (`colour.primary-soft`, half dot), **Unknown** (`colour.recessed`, hollow dot). Ink text on all three.
- **Form field:** label above in `font.body` 600, `colour.surface` fill, 1px `colour.field-border`, `radius.button`, at least 44px tall. Errors in words under the field.
- **Link:** `colour.ink` text with an underline in `colour.secondary`, which is ink in the CoEngineers system.
- **Focus:** 3px `colour.focus` outline, 3px offset, on every button, link and field.
- **Band:** `colour.band` with `colour.canvas` text. At most one per page, for one statement.

## Logo

The wordmark is "Chilli Community" set in Space Grotesk, "Chilli" in orange and "Community" in ink, the same pattern as the CoEngineers "Co". It is saved as shapes, so it looks the same in every tool, upload and email. The mark is a single chilli pod with its stem, orange on an ink tile: no face, nothing that vanishes at 24px. PNG copies (the mark 512px square, the wordmark 512px tall, transparent) are for tools that cannot take SVG.

- Wordmark: `brand/logo-wordmark.svg`, "Chilli Community" set in `font.display` 600. "Chilli" in `colour.primary`, "Community" in `colour.ink`. Orange here is part of the logo; it never carries other text.
- Mark: `brand/logo-mark.svg`, a single chilli pod with its stem in `colour.primary` on a `colour.ink` tile with rounded corners (an ink tile, so it never reads as a CoEngineers mark). For one-colour print, the pod in `colour.ink` on `colour.canvas`, with no tile. For small places: profile pictures, favicons, the corner of a slide.
- Clear space: at least the height of the wordmark's capital letters on every side.
- Smallest size: wordmark 96px wide on screen, 25mm in print; mark 24px.
- On `colour.band`: "Chilli" stays `colour.primary` (7.5:1 on the band) and "Community" goes `colour.canvas`. The mark goes on the band as it is; the orange pod carries it.
- Never stretch, outline, shadow, recolour outside these colours, or set the name in another typeface.

## Imagery

- Use: phone photos in real homes: kitchen windowsills, balconies, back gardens, a greenhouse bench
- Use: the real kit: black plastic pots, canes and twine, compost on newspaper, a watering can
- Use: plants as they are, leggy or dropping a leaf, photographed from the same spot week by week
- Use: hands at work: sowing, tying in, picking, chopping
- Use: food as it comes out of the pan, on the plate it was served on, in daylight
- Never: styled cookbook shots, props and studio light
- Never: stock photos of any kind
- Never: doodle cards, cartoon chillies or anything childish
- Never: flames, fire and heat-challenge clichés
- Never: a generated picture standing in for a member, a harvest or a result

- Real photos first: the founder's own, from their customers' real world.
- A generated image only ever sets a scene, is captioned "Illustrative", and never stands in for evidence (a customer, a result, a product in use).
- Photos sit on `colour.surface` stages with `radius.image`. Crop for the subject; never add filters or overlays that change what is real.
- Every image that carries meaning has alt text.
- Where things stand (30 September 2026): one real photo, Priya's own windowsill. The other two photos on the brand kit are illustrative stand-ins until her own replace them. A first cooked dish is still to come.

## Voice and words

Decided, Priya, 30 September 2026: kept as drafted.

- Plain, warm British English, the way you would say it at the windowsill: short sentences, plain words.
- Every tip is something a beginner can do this week, with what they already have.
- Honest when things go wrong: leggy plants, dropped flowers, a batch that failed.
- Warm and a bit dry. Never gushing, never cheerleading.
- Real over polished: say what happened and show the real photo.
- Never promise results. Say what is decided, what is being tested and what is not known yet.

- Words we use: grow, pot, windowsill, pod, this week, try, cook, share, real
- Words we avoid: hack, superfood, journey, game-changer, unlock, amazing, foodie, hottest ever
- British English. No em dashes. No exclamation-mark cheerleading.

## Do and don't

| Do | Don't |
|---|---|
| Use the CoEngineers tokens exactly as they are | Change a CoEngineers value for Chilli: the case study and videos are built on them |
| Use orange for the one thing that matters on a page: the main button | Set orange as text (it is 2.2:1 on paper), wash a section in it, or use it for decoration |
| Use leaf and chilli for small details: a tag, a plant label, a detail in a drawing | Use leaf or chilli for a button, a fill behind text, a status, or as big blocks side by side |
| Show real phone photos from real homes | Use styled cookbook shots, stock photos or cartoon chillies |
| Caption every stand-in or generated picture "Illustrative" | Let a generated picture stand in for a member, a harvest or a result |
| Show status in words: Decided, Testing, Unknown | Show status by colour alone |
| Use the Chilli wordmark and pod mark on Chilli pages | Put the CoEngineers wordmark on a Chilli page, or set the Chilli name in another typeface |
| Use two typefaces: Space Grotesk and Inter | Add a third typeface for labels or figures |

## Changes

- 23 September 2026: first version, the Windowsill direction (chilli red and leaf green, Bricolage Grotesque). Replaced the same day, see below.
- 23 September 2026: replaced at Priya's direction. "chilli community should be similar brand kit to coengineers as that's what we've built against so far", then, asked how close, "Coengineers exactly as we've already done the case study and base videos", and "Maybe with a few extra bits but needs to be similar or it will bork all our old assets". Every CoEngineers token is now used unchanged. Chilli keeps its own wordmark (now in Space Grotesk, "Chilli" in orange), a pod mark in orange on ink, and two extra colours for small details (Testing). The first draft's files stay in the history only.
- 30 September 2026 (Week 4): Priya confirmed the feel (warm, homegrown, calm), the colours with the two extras, the voice rules and the one accent with one job (the main button). Changed: small labels move from the third typeface to Inter, so Chilli uses two typefaces. Added the one-sentence reason for the look, with Priya's own words. Contrast pairs re-measured by code. Priya's own windowsill photo added to the brand kit.
