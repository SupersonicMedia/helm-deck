# HELM Interactive Investor Deck

An interactive, mobile-first investor pitch deck for HELM — a luxury hospitality marketplace paired with an agentic AI event planner. Built with Astro + Tailwind CSS.

## Tech Stack

- **Framework:** Astro
- **Styling:** Tailwind CSS + custom CSS (glassmorphism, animations)
- **Fonts:** Cormorant Garamond (headings), Poppins (body), Rubik (accent)
- **Libraries:** Swiper.js (mobile carousels)
- **Deployment:** Static site

## Project Structure

```
src/
  components/     # Individual slide components (17 total)
  layouts/        # Base HTML layout with fonts, Swiper, animations
  pages/          # index.astro — assembles all slides
  styles/         # global.css — design system, snap scrolling, reusable classes
public/
  images/         # All static assets (logos, photos, feature mockups)
HELM/
  HELM - 2026 Deck.pdf   # Source pitch deck PDF
  Background+Shadow*.png  # Feature mockup images
assets/
  images/         # Source logo files (cropped variants)
```

## Slide Order

| # | Component | Label |
|---|-----------|-------|
| 0 | Hero | HELM |
| 1 | Challenge | Challenge |
| 2 | AIPowered | Solution |
| 3 | WhyHelm | Why HELM |
| 4 | ProductExperience | Product |
| 5 | MarketOpportunity | Market |
| 6 | Founders | Founders |
| 7 | OperatingTeam | Team |
| 8 | RevenueStreams | Revenue |
| 9 | Economics | Growth Model |
| 10 | SubscriptionEconomics | Subscriptions |
| 11 | EventScenarios | Events |
| 12 | GoToMarket | GTM |
| 13 | Roadmap | Roadmap |
| 14 | UseOfFunds | Funds |
| 15 | Video | Video |
| 16 | ThankYou | Thank You |

## Key Features

- **Snap scrolling:** CSS `scroll-snap-type: y mandatory` for full-screen slide transitions
- **Bottom navigation:** Dot indicators, slide labels, and arrow buttons via DeckNav
- **Mobile-first:** Swiper carousels for content-heavy slides (AI-Powered, Founders, Operating Team)
- **Stacked layouts:** Revenue Streams and Event Scenarios stack vertically on mobile
- **Scrolling marquees:** Hero and Thank You pages feature auto-scrolling photo strips
- **Scroll animations:** IntersectionObserver-powered fade/scale entrance animations
- **Animated counters:** Number counters with eased animation on scroll

## Development

```bash
npm install
npx astro dev    # http://localhost:4321
npx astro build  # Production build
```
