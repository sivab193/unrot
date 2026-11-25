---
name: Obsidian Signal
colors:
  surface: '#121318'
  surface-dim: '#121318'
  surface-bright: '#38393f'
  surface-container-lowest: '#0d0e13'
  surface-container-low: '#1a1b21'
  surface-container: '#1e1f25'
  surface-container-high: '#292a2f'
  surface-container-highest: '#34343a'
  on-surface: '#e3e1e9'
  on-surface-variant: '#bdc8d1'
  inverse-surface: '#e3e1e9'
  inverse-on-surface: '#2f3036'
  outline: '#87929a'
  outline-variant: '#3e484f'
  surface-tint: '#7bd0ff'
  primary: '#8ed5ff'
  on-primary: '#00354a'
  primary-container: '#38bdf8'
  on-primary-container: '#004965'
  inverse-primary: '#00668a'
  secondary: '#c0c1ff'
  on-secondary: '#1000a9'
  secondary-container: '#3131c0'
  on-secondary-container: '#b0b2ff'
  tertiary: '#ffc176'
  on-tertiary: '#472a00'
  tertiary-container: '#f1a02b'
  on-tertiary-container: '#613b00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c4e7ff'
  primary-fixed-dim: '#7bd0ff'
  on-primary-fixed: '#001e2c'
  on-primary-fixed-variant: '#004c69'
  secondary-fixed: '#e1e0ff'
  secondary-fixed-dim: '#c0c1ff'
  on-secondary-fixed: '#07006c'
  on-secondary-fixed-variant: '#2f2ebe'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb960'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#121318'
  on-background: '#e3e1e9'
  surface-variant: '#34343a'
typography:
  headline-xl:
    fontFamily: Geist
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.03em
  headline-xl-mobile:
    fontFamily: Geist
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.025em
  headline-lg:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 30px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 26px
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 22px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
    letterSpacing: -0.005em
  body-md:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 20px
    letterSpacing: 0.005em
  label-md:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.04em
  label-sm:
    fontFamily: Geist
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.06em
  code-inline:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-sm: 0.75rem
  margin: 1rem
  margin-tablet: 1.5rem
  space-2xs: 0.125rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-base: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
  space-2xl: 3rem
---

## Brand & Style

The design system establishes a high-precision, distraction-free environment engineered specifically for deep technical journalism, engineering dispatches, and real-time tech industry intelligence. Its aesthetic merges modern ultra-minimalism with high-contrast tactical cues: void-like dark slate surfaces, surgical typography, and controlled bursts of electric luminescence.

The target audience consists of software architects, founders, technical investors, and engineering leaders who demand signal over noise. The interface avoids frivolous ornament, skeuomorphic noise, or decorative distraction. Instead, it evokes absolute focus, technical sophistication, and calm authority. Interactions are immediate, borders are laser-sharp, and content readability remains paramount across extended mobile reading sessions.

## Colors

The palette operates on a strict pitch-to-slate hierarchy designed to reduce optical fatigue on OLED and high-density mobile displays while directing cognitive attention to curated content.

- **Canvas & Surface Tiering:**
  - Base canvas (`#090A0F`): Deep obsidian-slate base establishing maximum contrast against typography.
  - Surface-1 / Cards (`#12141C`): Recessed elevated background for stream cards, article feeds, and modal backdrops.
  - Surface-2 / Overlays (`#1B1E2B`): Tertiary containers, floating navigation headers, bottom sheets, and active states.
  - Structural Divider (`#242838`): Hairline boundary color delivering structural isolation without visual weight.

- **Accents:**
  - Electric Cyan (`#38BDF8`): Primary dynamic accent reserved for read progress indicators, live breaking alerts, primary interactive triggers, and targeted text selections.
  - Cobalt Indigo (`#6366F1`): Secondary accent designating system status, categorical tags, analytics metrics, and deeper contextual anchors.

- **Monochrome & Text Hierarchy:**
  - High-Emphasis Content: `#F8FAFC` (95% contrast ratio against deep canvas).
  - Mid-Emphasis Body: `#94A3B8` (relaxed reading value for long-form consumption).
  - Low-Emphasis Meta & Microcopy: `#64748B`.

## Typography

The typographic hierarchy is split intentionally between **Geist** for crisp, architectural headlines and functional labels, and **Inter** for sustained readability within long-form technical reports.

- **Headline System:** Set tight with subtle negative tracking (`-0.015em` to `-0.03em`) to deliver a dense, editorial tech atmosphere. Headings above 24px automatically drop down to optimized mobile equivalents (`headline-xl-mobile`) to prevent awkward single-word wrapping on narrow devices.
- **Editorial Reading System:** Long-form article text relies on `body-lg` (18px) set at a relaxed 28px line height. Body text color is balanced at `#94A3B8` to diminish ocular glare in high-contrast dark environments.
- **Labels & Micro-Data:** Rendered in `Geist` with uppercase styling and expanded tracking (`+0.04em` to `+0.06em`) for timestamps, category metadata, ticker symbols, and read-time markers. Inline code and technical identifiers use monospaced sizing pinned directly to the x-height of surrounding body typography.

## Layout & Spacing

The layout model is driven by an 8-point base grid (supplemented by 4-point micro-increments), built primarily for high-density mobile ergonomics with seamless transitions to tablet reading canvases.

- **Mobile Viewports (<640px):** Single-column dynamic flow anchored by a fixed `1rem` (16px) outer margin. Article feeds utilize full-bleed separators or edge-to-edge modular cards with tight internal gutters (`0.75rem`).
- **Tablet/Foldable Viewports (640px - 1024px):** Dual-pane master-detail split (feed list on the primary rail at 360px fixed width, continuous article reader occupying the remaining space) with `1.5rem` canvas margins.
- **Reading Ergonomics:** Main editorial text blocks are clamped to a strict maximum width of `65ch` to preserve optimal eye-tracking speed. Vertical flow prioritizes generous section gaps (`space-xl` to `space-2xl`) between article chapters, paired with compact vertical margins (`space-xs` to `space-sm`) inside metadata headers.

## Elevation & Depth

Visual hierarchy abandons traditional drop shadows in favor of a **tonal surface layering system paired with razor-sharp 1px boundary lines**.

- **Level 0 (Canvas Base):** Pinned at `#090A0F`. Houses bottom-level page containers and deep article scroll canvases.
- **Level 1 (Card & Content Blocks):** Pinned at `#12141C` with a continuous `1px solid #242838` boundary. Elevated slightly above the canvas to organize continuous content modules.
- **Level 2 (Persistent Chrome & Floating Bars):** Tab navigation, floating quick-action docks, and sticky headers use `#12141C` rendered at 80% opacity with a `16px` backdrop-filter blur (`backdrop-filter: blur(16px)`). Bound by a bottom/top border of `1px solid #242838`.
- **Level 3 (Modals & Sheet Drawers):** `#1B1E2B` layered with a high-diffusion, dark-slate glow: `box-shadow: 0 20px 40px -15px rgba(0, 0, 0, 0.7), 0 0 0 1px #242838`.
- **Focus & Live State Glow:** High-priority items (breaking updates, real-time live feeds) employ a subtle accent halo: `box-shadow: 0 0 12px -2px rgba(56, 189, 248, 0.25)`.

## Shapes

The interface embraces a precise, structural architectural shape language with deliberate pill exceptions for rapid status recognition:

- **Structural Elements (Cards, Panels, Text Inputs):** Enforce `roundedness: 1` (`0.25rem` / 4px on small containers, reaching `0.5rem` / 8px for outer cards and bottom sheet corners). Corners are crisp, mechanical, and disciplined.
- **Categorical & Metadata Badges:** Strictly pill-shaped (`9999px` border-radius). Badges float as organic metadata units against the hard-edged, technical geometry of cards and image modules.
- **Interactive Buttons:** Primary and tertiary utility buttons utilize standard `rounded-sm` (4px) or `rounded-md` (8px) geometries, maintaining alignment with structural boundaries rather than soft consumer aesthetics.

## Components

- **Buttons:**
  - *Primary Action:* Solid `#38BDF8` background with `#090A0F` bold typography (`Geist`, 13px, weight 600). Radius: 6px. On press: scale transform `0.98` with luminance shift to `#7DD3FC`.
  - *Secondary / Ghost:* Transparent fill, `1px solid #242838`, text in `#F8FAFC`. Active state: background `#1B1E2B`, border `#38BDF8`.
  - *Icon Utility (Bookmark, Share, Font Size):* 36x36px square with 4px radius, `#12141C` background, `#94A3B8` icon color, transitioning to `#38BDF8` on trigger.

- **Pill Badges:**
  - *Category Tags:* Fully rounded pills (`border-radius: 9999px`), padding `2px 8px`. Slate background `#1B1E2B`, `1px solid #242838`, label in `Geist` 10px uppercase `#94A3B8`.
  - *Live / Breaking Signal:* Background `rgba(56, 189, 248, 0.1)`, `1px solid rgba(56, 189, 248, 0.4)`, text `#38BDF8`. Includes a 6px pulsing electric cyan indicator dot.

- **Feed Cards:**
  - Background `#12141C`, border `1px solid #242838`, radius 8px. Internal padding of 14px.
  - Image thumbnails: 16:9 aspect ratio, 4px inner radius, masked with a 5% inner linear black gradient to maintain contrast.

- **Input Fields (Search & Filters):**
  - Height 40px, background `#12141C`, border `1px solid #242838`, text `#F8FAFC`, placeholder `#64748B`. Focused state: border transitions immediately to `#38BDF8` without outer ring bloom.

- **Checkboxes & Segment Controls:**
  - Checkboxes: 16x16px boxes with a 2px corner radius. Unchecked: `1px solid #242838`. Checked: `#38BDF8` background with dark tick icon.
  - Segment Controls: Segmented pill container (`#12141C`, `1px solid #242838`), active indicator sliding pill in `#1B1E2B` with crisp `#38BDF8` typography.

- **Reading Progress Bar:**
  - Ultra-thin 2px persistent track pinned to the top navigation boundary. Filled dynamically via `#38BDF8` with a forward glowing edge.

- **Micro-interactions & Code Callouts:**
  - In-article code blocks: `#090A0F` fill with `1px solid #242838`, horizontal scroll with hidden scrollbar, accompanied by a top-right 1-click copy icon button.