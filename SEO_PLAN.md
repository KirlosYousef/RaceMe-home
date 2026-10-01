# RaceMe website SEO plan

**Status:** implemented in the static site. The site is served from the existing custom domain, `https://www.raceme.top/`, through GitHub Pages. The current Apple listing and app registration flow already link to the legal-page URLs in this repository; those exact paths are retained.

## Positioning and search intent

RaceMe is a social running app built around live competition. The clearest search promise is: **turn a run into a race with a friend, another runner, or your own previous result.** Keep that message consistent across the website, App Store listing, and share previews.

The groups below are search-intent hypotheses, not claimed search-volume data. Validate them in Search Console and App Store Connect after launch.

| Intent | Natural phrases to cover | Page or section |
| --- | --- | --- |
| Branded | RaceMe, RaceMe running app, RaceMe run with friends | Home page title, H1, app schema, footer |
| Race friends | running app to race friends, running challenge app, compete with friends while running | Home hero, head-to-head and friends feature cards, FAQ |
| Live competition | live running race app, real-time running competition, race another runner | Home hero, live-match feature, how it works |
| Personal improvement | run against your personal best, running personal-record challenge | Race-yourself feature card and FAQ |
| Route and distance | GPS running race, choose a running distance, running track challenge | Track-selection card, route privacy explanation |
| Apple devices | running app for iPhone and Apple Watch, Apple Watch race progress | Hero, Watch section, compatibility FAQ, App Store CTA |
| Trust and support | RaceMe privacy policy, RaceMe location privacy, RaceMe terms, RaceMe support | Privacy, terms, and contact pages |

Use these phrases as clear descriptions of features, never as a repeated keyword list. Do not claim race accuracy, fitness outcomes, global scale, awards, or user ratings that are not supported by the product and current public listing.

## Implemented on-page and technical SEO

- **Search-focused first screen:** one descriptive H1, a concise product explanation, feature cues visible without scrolling, and a direct App Store call to action.
- **Distinct page metadata:** unique descriptive title and meta description on the home, privacy, terms, and contact pages. Each page declares its own canonical URL on the existing HTTPS `www.raceme.top` domain.
- **Structured data:** the home page describes the site as `WebSite` and the iOS app as `MobileApplication`, with the public App Store link, supported OS information, app category, and free download offer. No review or rating data is fabricated. Google can choose whether to show enhanced search details; structured data is not a ranking or rich-result guarantee.
- **Crawl paths:** `robots.txt` allows crawling and points to `sitemap.xml`. The sitemap lists the canonical home, policy, terms, and contact URLs. The existing custom-domain `CNAME` is preserved.
- **App Store continuity:** `privacy_policy.html` and `terms_and_conditions.html` remain the exact paths linked by the current app and public App Store listing. The site footer, registration flow, and legal pages can continue to use those URLs.
- **Share previews:** Open Graph and X card metadata use a branded social image, an accurate title, a useful summary, and the canonical page URL.
- **Image accessibility and discovery:** descriptive file names and alt text explain each RaceMe screen and feature. Below-the-fold images lazy-load; the live-race hero image is prioritized.
- **Mobile and performance foundation:** static HTML, locally hosted fonts, compressed JPEG artwork, no client framework, no third-party marketing scripts, and no analytics cookies on the website. The layout supports reduced-motion preferences, keyboard focus, semantic navigation, and mobile screens.
- **Useful internal links:** primary navigation connects features and legal paths; the App Store destination is linked directly and consistently.

## Content and App Store alignment

The app’s public listing is **RaceMe: Run with Friends!** and describes live races, friend challenges, personal-best competition, track choices, Apple Watch, chat, rewards, and leaderboards. The landing page leads with the same supported themes and uses current RaceMe app screens and store artwork.

For the next App Store Connect metadata review:

1. Keep the product name and subtitle readable and aligned with the core “run with friends / live running races” intent.
2. Use the keyword field for distinct, relevant terms rather than repeating words already present in the title and subtitle. Avoid competitor names.
3. Keep the first three store screenshots focused on live head-to-head racing, friend challenges, and racing your previous best; use actual current UI and disclose paid features when shown.
4. Confirm the App Store privacy answers and linked privacy policy against the current SDKs, analytics events, location flow, and subscription providers.
5. Keep the website’s direct App Store URL current if the listing changes.

The website does not change App Store Connect metadata. Apple’s public listing was checked when this site was prepared: [RaceMe on the App Store](https://apps.apple.com/us/app/raceme-run-with-friends/id1514432749).

## Launch and measurement plan

1. **After the Pages update completes:** confirm `https://www.raceme.top/`, `/privacy_policy.html`, `/terms_and_conditions.html`, and `/sitemap.xml` resolve over HTTPS. Preserve the `www` canonical host and current App Store policy links.
2. **Search Console:** verify the `raceme.top` domain property using DNS access, submit `https://www.raceme.top/sitemap.xml`, and inspect the canonical URLs. This repository cannot complete DNS verification for the owner.
3. **First 2–4 weeks:** monitor indexing, impressions, clicks, and search phrases by page. Separate branded and non-branded queries. Fix crawl or canonical issues before changing copy.
4. **Conversion:** compare Search Console landing-page traffic with App Store product-page views and downloads in App Store Connect. Add campaign links only when the matching Apple campaign setup is available.
5. **Content:** prioritize one genuinely useful answer page at a time, such as “How to race a friend in RaceMe” or “How RaceMe uses location during a race.” Publish only when it answers a real user question with app-accurate detail; avoid thin pages made only to target keywords.
6. **Iteration:** after a meaningful query sample exists, refine one headline or feature description at a time. Do not infer success from a ranking snapshot or a small number of clicks.

## Search guidance sources

- [Google Search Central: title links](https://developers.google.com/search/docs/appearance/title-link)
- [Google Search Central: snippets and meta descriptions](https://developers.google.com/search/docs/appearance/snippet)
- [Google Search Central: software app structured data](https://developers.google.com/search/docs/appearance/structured-data/software-app)
- [Google Search Central: canonical URLs](https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls)
- [Google Search Central: crawling and indexing](https://developers.google.com/search/docs/crawling-indexing)
