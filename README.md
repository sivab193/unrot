# Unrot

**Unrot** is a minimal, high-signal tech news, opportunity radar, and developer deal discovery application built around the **Obsidian Signal** design system.

This repository contains the complete Stitch UI/UX prototypes, design system specification, visual assets, and seed deal content ready for **Google AI Studio** to connect and build out the full interactive application.

---

## Repository Contents

All extracted design assets live under [`stitch_minimal_tech_news_app/`](./stitch_minimal_tech_news_app):

### 1. Design System
- [`stitch_minimal_tech_news_app/obsidian_signal/DESIGN.md`](./stitch_minimal_tech_news_app/obsidian_signal/DESIGN.md) — Complete **Obsidian Signal** design system specification:
  - **Palette:** Pitch-to-slate dark hierarchy (`#090A0F` / `#121318` base canvas, `#12141C` / `#1E1F25` surfaces, `#242838` 1px structural dividers) with Electric Cyan (`#38BDF8`), Cobalt Indigo (`#6366F1` / `#C0C1FF`), and Amber (`#FFC176`) accents.
  - **Typography:** `Geist` (headlines & uppercase labels), `Inter` (long-form editorial reading), and `JetBrains Mono` (promo codes, technical tags, inline code).
  - **Components & Layout:** 8pt spacing grid, mobile-first layout (`<640px` single-column, `640px–1024px` master-detail), 1px tonal borders, pill category badges, reading progress bar, and copy-to-clipboard terminal widgets.

### 2. Screen Prototypes (`code.html` + `screen.png`)
Each screen folder includes a Tailwind CSS HTML prototype (`code.html`) and a visual reference render (`screen.png`):

| Screen | Folder | Purpose |
| --- | --- | --- |
| **Signal Feed** | [`signal_feed/`](./stitch_minimal_tech_news_app/signal_feed) | Editorial tech news & dispatches feed with category filter pills, audio briefing mini-player, featured *Top Signal* card, upvotes/comments/bookmarks, and bottom navigation (`Feed`, `Topics`, `Saved`, `Profile`). |
| **Article Reader** | [`article_view/`](./stitch_minimal_tech_news_app/article_view) | Distraction-free long-form reader with sticky top reading progress bar, author row, font size switcher, *Listen to Article* audio pill, executive brief, and technical callouts. |
| **Signal Reels — Deals & Tech** | [`signal_reels_deal_tech_feed/`](./stitch_minimal_tech_news_app/signal_reels_deal_tech_feed) | TikTok/Reels-style vertical snap-scroll feed (`Loop // Signal Snaps`) showcasing AI/dev tool credits and deals with 1-tap copy toast, upvote stack, and bottom nav (`Feed`, `Radar`, `Claimed`, `Profile`). |
| **Signal Reels — YC, Grants & Hackathons** | [`signal_reels_yc_grants_hackathons/`](./stitch_minimal_tech_news_app/signal_reels_yc_grants_hackathons) | Vertical snap-scroll feed (`Signal // Reels Feed`) with horizontal filter tabs for YC batch spotlights, non-dilutive research grants, and global hackathons. |
| **Deal Claim Terminal** | [`deal_claim_terminal/`](./stitch_minimal_tech_news_app/deal_claim_terminal) | Bottom-sheet redemption terminal (`Loop // Signal Details`) with live social proof ticker, urgency countdown, copyable promo code ticket box, and 30-second TL;DR expandables. |

### 3. Visual Assets & Seed Data
- **Vertical 9:16 Reels Backgrounds:**
  - [`vertical_9_16_futuristic_tech_aesthetic_background_for_instagram_reels_card/screen.png`](./stitch_minimal_tech_news_app/vertical_9_16_futuristic_tech_aesthetic_background_for_instagram_reels_card/screen.png)
  - [`vertical_9_16_cyber_hackathon_arena_stage_background_dark_obsidian_theme_with/screen.png`](./stitch_minimal_tech_news_app/vertical_9_16_cyber_hackathon_arena_stage_background_dark_obsidian_theme_with/screen.png)
  - [`vertical_9_16_high_tech_global_funding_grant_matrix_theme_abstract_world/screen.png`](./stitch_minimal_tech_news_app/vertical_9_16_high_tech_global_funding_grant_matrix_theme_abstract_world/screen.png)
- **Seed Content Reference:**
  - [`stitch_minimal_tech_news_app/extracted_text_from_https_resourify.com.md`](./stitch_minimal_tech_news_app/extracted_text_from_https_resourify.com.md) — Curated software, AI credits, student discounts, and startup deal items to populate initial mock/seed datasets.

---

## Building with Google AI Studio

When connecting this repository in **Google AI Studio**, use the following guidance to scaffold the production app at the repository root while preserving the design system:

1. **Follow `DESIGN.md` strictly:** Configure Tailwind CSS with the exact **Obsidian Signal** color tokens, `Geist` / `Inter` / `JetBrains Mono` font families, 1px `#242838` borders, and Material Symbols Outlined icons.
2. **Core Navigation & Views:**
   - **Feed (Signal Feed & Signal Reels toggle/modes):** Editorial tech dispatches (`signal_feed`) and vertical snap-scrolling reels (`signal_reels_deal_tech_feed` & `signal_reels_yc_grants_hackathons`).
   - **Article Reader (`article_view`):** Accessible from any editorial dispatch card, with live scroll progress tracking, font size controls, and audio summary playback state.
   - **Radar / Topics & Saved / Claimed:** Category filtering (AI, Grants, Hackathons, Dev Deals, YC), bookmarked articles, and claimed promo codes.
   - **Deal Claim Terminal (`deal_claim_terminal`):** Slide-up modal/sheet triggered from deal reels with 1-click promo code copy, toast confirmation, and expandable TL;DR steps.
3. **Seed Data:** Populate deals, promo codes, grants, hackathons, and tech dispatches using the structured content in `extracted_text_from_https_resourify.com.md` and the HTML prototypes.
