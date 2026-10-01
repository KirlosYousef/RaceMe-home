# RaceMe Home

Static landing site for the RaceMe iOS and Apple Watch app, published from this repository with GitHub Pages at [www.raceme.top](https://www.raceme.top/).

## Pages

- Home: `index.html`
- Privacy policy: `privacy_policy.html`
- Terms and conditions: `terms_and_conditions.html`
- Support: `contact.html`
- SEO implementation plan: `SEO_PLAN.md`

The privacy and terms file paths match the links already used by the app and App Store listing. The App Store download button links to [RaceMe: Run with Friends!](https://apps.apple.com/us/app/raceme-run-with-friends/id1514432749).

## Preview locally

Serve the repository root with any static file server. For example:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

## Publishing

GitHub Pages already publishes the `master` branch from the repository root with the custom domain in `CNAME`. The site has no build step or package dependencies. Keep that Pages source and the custom-domain file in place when publishing future updates.
