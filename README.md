[README.md](https://github.com/user-attachments/files/31339276/README.md)


# Handoff: Spotlight Live OS — The Rainbow Cactus

## Overview

Spotlight Live OS is a live-event management platform for **The Rainbow Cactus**, a drag show
venue at 475 S. Lynnhaven Road, Virginia Beach, VA, running nightly events with roughly 8+
bartenders on rotating shifts. It is intended to replace **Toast** (POS) and **Eventbrite**
(ticketing) with one system.

It is built and branded as a product of **SpotlightSearch.io** ("Powered by SpotlightSearch.io"),
white-labelled to the venue: the venue's identity leads, SpotlightSearch sits in the background.
The prototype also contains the client-facing **proposal** screens used to pitch the platform.

Five user roles are covered:

| Role | Scope |
| --- | --- |
| Owner | Money, payroll, analytics, compliance across the venue |
| Manager | Nightly operations: run of show, booking, scheduling, box office, POS, inventory, work orders, HR cases |
| Employee | Own shift, time clock, swaps, pay, and issue reporting |
| Performer | An **independent artist account** — bookings across many venues, of which the Cactus is one |
| Guest / Vendor | Public event listing, checkout, digital ticket; vendor purchase orders and receiving |

Two design decisions matter and should survive implementation:

1. **The performer is not an employee of the venue.** A performer's account belongs to the
   performer and spans venues. The Cactus appears as one *venue portal* inside their account.
   Performers can apply to open calls at other venues, hold contracts with several venues, and
   carry the same reporting rights at every venue they work.
2. **Reporting is a first-class system, not a form.** Maintenance work orders and HR/harassment
   cases share one intake with three disclosure modes — **named, confidential, anonymous** — and
   each mode has different routing and visibility rules. This is the most sensitive part of the
   product; see *Reporting & disclosure* below.

## About the design files

The files in this bundle are **design references created in HTML** — prototypes that show the
intended look, structure, copy, and click behavior. They are **not production code to copy
directly.**

The task is to **recreate these designs in the target codebase's existing environment** (React,
Vue, Next, SwiftUI, native, whatever is in use), using its established routing, component
library, state management, and data layer. If no codebase exists yet, choose the framework most
appropriate for the product (a multi-tenant web app with a POS surface and mobile-friendly
employee/guest views) and implement the designs there.

Specifically, do not ship as-is:

- All data in the prototype is **hard-coded static markup**. Every table row, metric, name, and
  dollar figure is illustrative.
- Navigation is a single client-side `page` state variable, not real routing.
- Styles are inline `style` attributes (a constraint of the prototyping environment). In
  production, use the codebase's styling approach and the design tokens listed below.
- The `_ds/` bundle is the SpotlightSearch design system compiled for the prototype. Treat it as
  the **visual specification**, not a dependency to install.

## Fidelity

**High-fidelity.** Colors, typography, spacing, copy, and interaction states are final-intent.
Recreate the UI closely, using the codebase's existing primitives where they exist. Where the
prototype and the codebase's design system disagree on a primitive (button height, input styling),
prefer the codebase primitive and keep the brand's color/type tokens.

Layout is designed for a **1440 × 900** desktop canvas. Responsive behavior below ~1100px was
**not** designed — see *Responsive* below.

---

## Global shell

Every screen except the guest-facing ones sits in the same two-column shell.

**Root:** `display:flex; min-height:100vh; background:#0C0E10; color:#EAF0F0;`
body font `Poppins`, base size `14.5px`.

### Sidebar (left rail)

- `width: 250px; flex: none; height: 100vh; position: sticky; top: 0;`
- `background:#0C0E10; border-right:1px solid #1B1F22`
- Vertical stack: brand block → scrolling nav → Hedy AI row → "Powered by" row.

**Brand block (venue context)** — `padding: 22px 22px 18px`
- `THE RAINBOW` — Poppins 800, 11px, letter-spacing `.26em`, `#8A939A`
- `CACTUS` — Poppins 800, 27px, letter-spacing `.02em`, each letter a different hue:
  `C #E8705A`, `A #E3B85F`, `C #F2D06B`, `T #2FE0C4`, `U #7CC2B7`, `S #9BA8E8`
- `VIRGINIA BEACH` — IBM Plex Mono 500, 8.5px, letter-spacing `.24em`, uppercase, `#5B646B`

**Brand block (performer context)** — the SpotlightSearch inline logo (38px) plus
`ARTIST ACCOUNT / KAMILLA BELLADONNA` in mono 8.5px, `.18em`, `#5B646B`. The venue lockup is
replaced entirely, because the performer's account is not the venue's.

**Nav** — `flex:1; overflow-y:auto; padding: 4px 12px 20px;` groups separated by `gap: 14px`,
items by `gap: 2px`.
- Group label: mono 500, 9px, letter-spacing `.22em`, uppercase, `#4A5257`, `padding: 6px 10px 8px`
- Item: `padding: 9px 12px; border-radius: 8px; font-size: 13.5px;`
  transition `background 160ms, color 160ms`
  - default: `background: transparent; color: #8A939A`
  - active: `background: rgba(6,229,199,.10); color: #2FE0C4`

**Hedy AI row** — `border-top: 1px solid #1B1F22; padding: 14px 22px 18px`. A 26px circle with a
`1px solid #4A3C1E` border holding a 12px gold (`#C79A45`) spotlight glyph, the label `Hedy AI` at
13px `#C79A45`, and a right-aligned `ON` in mono 8px `.16em` `#5B646B`. Hedy AI is the assistant
layer; it is present but deliberately quiet.

**Powered-by row** — `POWERED BY` in mono 8px `#3A4046`, then the wordmark at Poppins 800 10px:
`Spotlight #5B646B` · `Search #2F8A80` · `.io #3A4046`.

### Main column

- `flex:1; min-width:0; height:100vh; overflow-y:auto;` (`id="ss-main"`; scroll resets to 0 on
  every navigation)

**Sticky page header** — `position:sticky; top:0; z-index:5; padding:18px 40px;`
`background: rgba(12,14,16,.94); backdrop-filter: blur(10px); border-bottom: 1px solid #1B1F22`.
Contains the page `<h1>` (Poppins 800, 30px, letter-spacing `-.02em`, `#EAF0F0`) on the left and
1–2 small buttons on the right.

**Page body** — `padding: 52px 40px 72px` for hero/marketing pages, tighter for dashboards;
content is centered with `max-width: 1180px` where it is prose-led. Hero surfaces carry the
brand's one permitted gradient, the **spotlight wash**:
`radial-gradient(120% 90% at 50% -20%, rgba(6,229,199,.10) 0%, transparent 55%)`.

### Card patterns

- **Standard card** — `background:#15181B; border:1px solid #23282C; border-radius:16px; padding:26px`
- **Inset row / well** — `background:#0F1214; border:1px solid #23282C; border-radius:10px; padding:12–14px`
- **Money card** — same as standard with `border-color: rgba(227,184,95,.30)`
- **Signal card** — same with `border-color: rgba(47,224,196,.24)`
- **Empty/upload state** — `background:#0F1214; border:1px dashed #3A4046; border-radius:10px`,
  13.5px `#5B646B`
- **Table** — CSS grid inside a card, e.g. `grid-template-columns: .9fr 1.1fr .7fr .7fr .8fr`.
  Header cells: mono 500, 9.5px, `.16em`, uppercase, `#5B646B`, `padding: 12px 26px` (first/last)
  or `12px 12px`. Body cells: 13.5px, `padding: 14px`, each cell carrying
  `border-top: 1px solid #23282C` (there is no `<tr>` — the grid draws its own rules).
  Numbers, times, and money in cells use IBM Plex Mono at 12.5px.
- **Status cell** — mono 500, 9.5px, `.12em`, uppercase; color carries the meaning:
  `#2FE0C4` positive/live/paid · `#E3B85F` needs action/money · `#8A939A` neutral/hold ·
  `#E8705A` critical.
- **Section kicker** — the design system `Kicker` component: mono uppercase eyebrow with an
  optional leading tick, tones `signal` (aqua), `money` (gold), `neutral`.

---

## Screens

36 screens, grouped exactly as the sidebar groups them. Screen keys are the prototype's `page`
state values and make reasonable route slugs.

### Proposal (client-facing pitch — not part of the shipped product)

| Key | Name | Purpose |
| --- | --- | --- |
| `cover` | Overview | Hero statement: "One Operating System For The Cactus." Prepared-for kicker, lede, headline metrics. Header actions: *Download PDF*, *Approve Pilot*. |
| `problem` | The Problem | Why Toast + Eventbrite + spreadsheets + group chats fail this venue. |
| `platform` | The Platform | Module map of everything the OS covers. |
| `integrations` | Integrations | Third-party surface: payments, e-signature, accounting, scheduling. |
| `migration` | Migration & Terms | Cutover plan, pricing, commercial terms. |

These can be dropped from the product build, or kept behind an internal/sales route.

### Owner

| Key | Name | Purpose |
| --- | --- | --- |
| `command` | Command Center | Single-glance venue health: tonight's revenue, ticket sales, labor %, open cases. |
| `financials` | Financials | Revenue by channel, cost of goods, settlements, gold money treatment throughout. |
| `payroll` | Payroll Runs | Approve and run payroll; per-employee hours, tips, deductions. |
| `analytics` | Venue Analytics | Trends across nights, events, performers, and door counts. |
| `compliance` | Compliance Vault | Licenses, insurance certificates, ABC compliance, expiry tracking. |

### Manager

| Key | Name | Purpose |
| --- | --- | --- |
| `tonight` | Tonight · Run of Show | The operational spine of the night: call times, set order, staff on, door status. |
| `booking` | Booking Calendar | Event calendar with holds and confirmations. |
| `scheduling` | Scheduling & Shifts | Build shifts for 8+ bartenders on rotation; publish, cover gaps, watch labor cost. |
| `boxoffice` | Box Office | Ticket inventory, comps, guest list, walk-up sales. |
| `bar` | Bar, Kitchen & POS | Point of sale: tabs, tickets, modifiers, tip handling. |
| `inventory` | Inventory | Counts, par levels, variance, low-stock signals. |
| `workorders` | Work Orders | Maintenance queue fed by staff and performer reports. |
| `cases` | HR Cases | Sensitive case queue with disclosure-aware visibility. |

### Employee

| Key | Name | Purpose |
| --- | --- | --- |
| `myshift` | My Shift | Tonight at a glance for one bartender/host: station, times, tasks. |
| `timeclock` | Clock & Checklists | Clock in/out plus opening/closing checklists. |
| `swaps` | Swaps & Availability | Offer, claim, and approve shift swaps; set availability. |
| `report` | Report an Issue | The intake form — see *Reporting & disclosure*. |
| `mypay` | My Pay & Tips | Hours, tips, pay stubs, next payday. |

### Performer · Artist Account

| Key | Name | Purpose |
| --- | --- | --- |
| `bookings` | My Bookings | All bookings across all venues in the network. |
| `opencalls` | Open Calls | Browse and apply to other venues' calls. |
| `venueportal` | Venue Portal · Cactus | Everything about this one venue: upcoming dates, payments from this venue, tonight's call time / set / dressing room / bill / music status, a *Needs You* action list, and *Raise Something Here* (report an issue, leave this venue). |
| `contracts` | Contracts | Contracts per venue, in states `SENT` → `READY TO SIGN` → `SIGNED`. |
| `settlements` | Settlements | Fee + tips per booking, in states `READY TO SIGN` → `PAID`. |
| `rider` | Rider & Media Kit | Technical rider, music, photos, bio — the performer's own asset, reused across venues. |

Illustrative values from the venue portal, which show the intended shapes: booking dates
`Sat 29 Aug` (Saturday Drag Show, 18:30, $650, `CONFIRMED`), `Wed 2 Sep` (What It Do?!, 21:30,
$300, `CONFIRMED`), `Sat 12 Sep` (Guest headliner support, 18:00, $800, `SIGN CONTRACT`),
`Sat 19 Sep` (18:30, $650, `HOLD`). Settlement rows pair a fee with tips ($650 + $284 tonight).

### Guest & Vendor

| Key | Name | Purpose |
| --- | --- | --- |
| `listing` | Event Listing | Public event page: lineup, times, ticket tiers. |
| `checkout` | Checkout | Ticket purchase — the Eventbrite replacement. |
| `ticket` | Digital Ticket | Post-purchase ticket with scannable code. |
| `purchasing` | Vendor Orders | Purchase orders to suppliers. |
| `receiving` | Receiving | Check deliveries against orders into inventory. |

Guest screens are the only ones a member of the public sees. They should be **mobile-first** in
implementation even though the prototype shows them at desktop width.

### Platform

| Key | Name | Purpose |
| --- | --- | --- |
| `door` | Door & Access | Scan tickets, count heads, manage capacity and ID checks. |
| `admin` | Admin & Roles | Users, roles, permissions, venue configuration. |

---

## Reporting & disclosure

The single most consequential flow. One intake, four categories, three disclosure modes.

**Categories** (`cat` state, default `harassment`): `maintenance`, `interpersonal`,
`harassment`, `guest`.
Selected chip: `background: rgba(6,229,199,.07); border-color: rgba(47,224,196,.38)`.
Unselected: `background:#0F1214; border-color:#23282C`.

**Disclosure modes** (`mode` state, default `anonymous`):

| Mode | Selected style | Meaning to build |
| --- | --- | --- |
| `named` | `bg rgba(6,229,199,.09)`, `border rgba(47,224,196,.42)`, `text #2FE0C4` | Reporter identity attached; normal routing and follow-up. |
| `confidential` | same | Identity known to the case system and a restricted recipient set, not to the subject or line managers. |
| `anonymous` | same, plus the explanation card gets `border: 1px solid rgba(47,224,196,.24)` | No identity stored. Follow-up happens through a claim code, not an account link. |

Each mode renders its own **"WHAT HAPPENS"** explanation card below the selector (mono 9.5px,
`.14em`, `#2FE0C4` heading). Do not collapse these into one generic paragraph — the differences
are the point, and the copy is a commitment to the reporter.

Implementation requirements the design implies:

- Anonymous reports must not be joinable back to a user record, session, or device. Do not log the
  submitting user id on the case row.
- Attachment upload states **"metadata is stripped on upload"** — strip EXIF/geotags server-side
  before storage, and do it for real.
- Category routes the case: `maintenance` → Work Orders queue; `interpersonal` / `harassment` →
  HR Cases queue with restricted visibility; `guest` → manager queue.
- Performers get the same intake at any venue they work (entry point on the venue portal), with
  routing to that venue's queues.
- The manager-side HR Cases screen must respect disclosure mode in what it renders — an anonymous
  case shows no reporter column.

## Interactions & behavior

- **Navigation.** Sidebar buttons set one `page` value; the main column scrolls to top on change.
  In production, use real routes per screen key so links and deep links work.
- **Nav transition.** `background 160ms, color 160ms` on nav items.
- **Hover.** Per the brand: lift 1px, outline picks up aqua. **Press:** `scale(.985)`.
  No bounce, no spring. Durations 120–420ms, `ease-out`.
- **Selection controls** (disclosure modes, categories) are single-select chip groups that swap
  background/border/text tokens as tabulated above.
- **Buttons** come from the design system: `primary` (aqua fill), `secondary` (outline),
  `ghost`, `money` (gold), sizes `sm` / `md` / `lg`, plus a `full` boolean for full-width.
- **States not designed.** Loading, empty, error, and form-validation states are absent from the
  prototype. Design/implement them using the tokens here: skeletons on `#0F1214`, error text
  `#E8705A`, dashed `#3A4046` for empty.
- **Live data.** Several screens present themselves as real-time (tonight's revenue, door counts,
  ticket sales). The brand treats aqua as the signal of live intelligence, so anything aqua should
  actually be live — poll or subscribe rather than render stale values in aqua.

## State management

The prototype holds three values; production needs far more, but these three map to real UI state:

| Prototype state | Default | Production equivalent |
| --- | --- | --- |
| `page` | `cover` | Route |
| `mode` | `anonymous` | Disclosure mode on the report form |
| `cat` | `harassment` | Category on the report form |

Server-side data domains the screens require: users & roles, employees, shifts & swaps, time
clock punches, payroll runs, performers (cross-venue), venues, bookings & holds, contracts,
settlements, events, ticket types & orders, tickets & scans, POS tabs & orders, menu & modifiers,
inventory items & counts, vendors & purchase orders, receiving records, work orders, HR cases &
disclosure records, compliance documents.

Because performers are cross-venue entities, model **performer ↔ venue as a relationship**
(booking, contract, settlement, portal access) rather than making performers children of a venue.
Multi-tenancy is a requirement, not a later addition — the platform is meant to be white-labelled
to other venues.

## Design tokens

**Ink & paper**

| Token | Value | Use |
| --- | --- | --- |
| Ink | `#0C0E10` | App background, sidebar |
| Card | `#15181B` | Card surfaces |
| Well | `#0F1214` | Inset rows, wells, inputs |
| Hairline | `#23282C` | Card borders, table rules |
| Hairline (sidebar) | `#1B1F22` | Sidebar borders |
| Text | `#EAF0F0` | Primary text |
| Text muted | `#8A939A` | Secondary text, inactive nav |
| Text dim | `#5B646B` | Mono labels, captions |
| Text faint | `#4A5257` | Nav group labels |
| Border faint | `#3A4046` | Dashed/empty states |
| Header glass | `rgba(12,14,16,.94)` + `blur(10px)` | Sticky headers |

**Signal & meaning** — usage ratio is a rule: ~70% neutral, 18% ink, **9% aqua, 3% gold**.

| Token | Value | Use |
| --- | --- | --- |
| Aqua (brand) | `#06E5C7` | Brand aqua; tints e.g. `rgba(6,229,199,.10)` |
| Aqua (interface) | `#2FE0C4` | Live/healthy/active state, instrumentation |
| Aqua tint | `rgba(47,224,196,.24 – .42)` | Signal borders |
| Gold (brand) | `#C79A45` | Money, Hedy AI accent |
| Gold (interface) | `#E3B85F` | Money figures, caution, needs-action |
| Critical | `#E8705A` | Critical status only |
| Teal | `#7CC2B7` / `#2F8A80` | Supporting tint, wordmark |
| Venue accent | `#F2D06B`, `#9BA8E8` | Cactus lockup letters only |

Status colors carry meaning. Never decorate with them.

**Typography** — two families only.

| Role | Spec |
| --- | --- |
| Display | Poppins 800, Title Case, letter-spacing `-.02em`. Hero 66px/.98 · page `h1` 30px/1 · section 34px/1.02 |
| Body | Poppins 400. Lede 19px/1.5 · body 14.5px/1.6 · table cell 13.5px · nav item 13.5px |
| Instrument | IBM Plex Mono 500, **always uppercase**, wide tracking. Table header 9.5px/`.16em` · status 9.5px/`.12em` · kicker 9.5px/`.14em` · nav group 9px/`.22em` · furniture 8–8.5px/`.16–.26em` · numbers in cells 12.5px |

All metrics, times, dates, money, and labels are mono and tabular. Money always carries the gold
treatment.

**Radius:** 8px (nav items, buttons) · 10px (wells, inset rows) · 12px (explanation cards) ·
16px (cards) · pill (buttons, badges). Never bubbly.

**Spacing:** 4-based rhythm. Recurring values: 2, 5–7, 9–10, 12, 14, 16, 18, 22, 26, 40, 52, 72.
Page gutter 40px; card padding 26px; card grid gap 16px.

**Elevation:** soft, cool, restrained. The signature light is the aqua glow
(`--glow-aqua`, `--glow-aqua-soft`), used sparingly, plus a gold glow in money contexts.

**Gradients:** one only — the spotlight wash
`radial-gradient(120% 90% at 50% -20%, rgba(6,229,199,.10) 0%, transparent 55%)`.
No other gradients.

**Scrollbars:** 10px, thumb `#23282C` at `border-radius:99px`, transparent track.

## Responsive

Designed at 1440 × 900 desktop only. Not designed, and needing design decisions:

- **Manager POS (`bar`) and door (`door`)** will be used on tablets in a dark, busy room. Hit
  targets should be ≥44px and contrast should hold at low screen brightness.
- **Employee screens** (`myshift`, `timeclock`, `swaps`, `report`, `mypay`) are phone-first in
  reality. The 250px sidebar should become a bottom bar or drawer.
- **Guest screens** (`listing`, `checkout`, `ticket`) are majority mobile traffic.

Flag these back for design rather than guessing at breakpoints.

## Assets

- **SpotlightSearch marks** — `_ds/.../assets/mark-aqua.svg`, `mark-gold.svg`, `mark-white.svg`,
  plus `favicon.png`. Aqua is primary; never recolor the primary aqua. Gold for money contexts.
- **Logo lockups** — via the design system `Logo` component (`lockup` / `horizontal` /
  `wordmark` / `inline` / `mark`, dark & light themes).
- **The Rainbow Cactus lockup** is drawn in type (Poppins 800, per-letter colors above), not an
  image. If the venue has a real logo file, it should replace this.
- **UI icons** — inline SVG at 1.5–2px stroke, matching **Lucide** geometry
  (`https://unpkg.com/lucide-static`). Lucide is a stand-in; the brand defines no UI icon set.
- **Fonts** — Poppins and IBM Plex Mono, loaded via Google Fonts in
  `_ds/.../tokens/typography.css`. Self-host in production.
- **No photography** is used in the prototype. The brand calls for cinematic, cool-toned, restrained
  real environments — never posed performers, film reels, or clapperboards. Any imagery added needs
  the venue's own photography.
- **`uploads/`** in the source project holds reference screenshots of the venue's current tools;
  they are not part of this bundle.

## Integrations to build (not yet designed in detail)

Named on the `integrations` screen and in the roadmap: **DocuSign** or equivalent e-signature for
performer contracts, a **payment processor** for ticketing and POS card present/not-present,
**payroll/tax filing**, **accounting export**, and scheduling. The contract and settlement screens
assume an e-signature round trip (`SENT` → `READY TO SIGN` → `SIGNED`) — wire the real states to
the provider's webhooks rather than local flags.

## Files in this bundle

| File | What it is |
| --- | --- |
| `Spotlight Live OS.dc.html` | The source prototype. Needs `support.js` and `_ds/` beside it. |
| `support.js` | Runtime for the prototype format. Not production code. |
| `_ds/` | Compiled SpotlightSearch.io design system: `tokens/{colors,typography,spacing,effects}.css`, `styles.css`, `_ds_bundle.js` (React primitives: Logo, SpotlightMark, Button, Kicker, Badge, Card, Gauge, Sparkline, Stat, FeedItem), `readme.md`. |
| `Rainbow Cactus Live Event OS.html` | **Start here.** Standalone single-file build — open directly in a browser, works offline, full navigation intact. |
| `README.md` | This document. |

To view: open `Rainbow Cactus Live Event OS.html` in any browser. Click through the sidebar to
reach all 36 screens.
