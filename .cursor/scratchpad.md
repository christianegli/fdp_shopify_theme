# Project Scratchpad
**Current Role:** Planner
**MVP Status:** Not Started
**GitHub Repo:** https://github.com/christianegli/fdp_shopify_theme
**Last Push:** 2025-06-13T09:15:00Z

## Background and Motivation
The client requests a redesign of the current Shopify theme to emulate the look and feel of Dior's official fashion site (https://www.dior.com/de_de/fashion?animate=true). The goal is to elevate the store's visual identity to match luxury brand standards and improve user perception and engagement.

## Research Findings
### Competitive Analysis
- **Dior (Reference Site):**
  - Clean, minimalist layout with significant white space
  - Elegant serif typography (e.g., custom "Dior" font) combined with modern sans-serif for UI elements
  - Large, high-resolution hero imagery & full-width videos
  - Sticky top navigation that expands into a full-screen mega-menu overlay
  - Subtle micro-interactions (fade-in animations, smooth scrolling)
  - Monochrome palette (black, white, light gray) with occasional accent colors
  - Grid-based product listing with generous spacing, hover-zoom effects, and concise info reveal
  - Emphasis on storytelling sections (Savoir-Faire, Editorial) using full-bleed imagery and rich media
  - Distraction-free footer with multilayered links in small type, tinted background

### User Pain Points (from typical premium-brand customers)
1. Current theme feels generic and does not convey luxury, reducing perceived product value.
2. Navigation is cluttered; customers struggle to discover collections quickly.
3. Visual storytelling is weak; limited use of immersive imagery and editorial sections.

### MVP Definition
Core functionality that must ship first to achieve Dior-like aesthetic:
- [ ] Global style overhaul: luxury typography (e.g., Playfair Display or similar serif plus clean sans-serif), monochrome palette, generous white space. **ESSENTIAL**
- [ ] Hero section on home page: full-width responsive image/video slider with fade transition. **ESSENTIAL**
- [ ] Simplified sticky header with logo left, centered menu trigger, right-aligned icons. **ESSENTIAL**
- [ ] Mega-menu overlay with two-column layout and large background image. **ESSENTIAL**
- [ ] Product grid redesign: larger thumbnails, hover zoom, price hidden until hover or subtle below image. **ESSENTIAL**
- [ ] Basic storytelling section template (full-bleed image + text overlay). **ESSENTIAL**

## Implementation Plan

### Phase 1: MVP (Core Functionality)
- [x] Task 0: Create GitHub repository and initialize project structure (README, ARCHITECTURE, DECISIONS, docs/).
  - Success: Repository exists, documentation scaffolding committed.  ✅
  - Priority: CRITICAL
- [ ] Task 1: Global style overhaul (typography, monochrome palette, spacing).  
  - Success: All theme pages load new fonts & color scheme without layout breakage.  
  - Priority: CRITICAL
- [ ] Task 2: Implement sticky header with compact logo/menu/utility icons plus full-screen mega-menu overlay.  
  - Success: Scroll-responsive header and overlay menu function across desktop & mobile breakpoints.  
  - Priority: CRITICAL
- [ ] Task 3: Home-page hero slider (full-width image/video, fade transition, mobile responsive).  
  - Success: Autoplay & swipe enabled; CLS < 0.1 on Lighthouse.  
  - Priority: CRITICAL
- [ ] Task 4: Product grid redesign with hover-zoom, enlarged thumbs, price reveal.  
  - Success: Collection & featured product sections adopt new grid with no Shopify Liquid errors.  
  - Priority: CRITICAL
- [ ] Task 5: Storytelling section template (full-bleed image + text overlay).  
  - Success: Section available in Shopify customizer with configurable image & text blocks.  
  - Priority: CRITICAL

### Phase 2: Enhancements
- [ ] Enhancement 1: Lazy-load animations for editorial sections.  
  - Success: Intersection Observer triggers fade-in without jank.  
  - Priority: NICE-TO-HAVE
- [ ] Enhancement 2: Custom cursor / subtle parallax effects.  
  - Success: Effects toggleable in theme settings; no performance regression.  
  - Priority: NICE-TO-HAVE
- [ ] Enhancement 3: Personalized recommendation carousel.  
  - Success: Recommender uses Shopify product recommendations API, passes accessibility tests.  
  - Priority: NICE-TO-HAVE
- [ ] Enhancement 4: Accessibility & dark-mode toggle.  
  - Success: WCAG AA contrast met; user can switch modes.  
  - Priority: NICE-TO-HAVE 