# Esports Arena Bracket Predictor

A mobile-friendly, installable esports tournament bracket app with a futuristic neon arena interface.

## Included features
- Organizer tournament creation for 4, 8, or 16 teams
- Team registration, color and tagline, updates and withdrawals
- Animated, horizontally navigable bracket with match winner selection
- Real-result view, model prediction and random upset simulation
- Monte Carlo championship odds (6,000 simulated finishes)
- Organizer team-rating controls
- Personal bracket picks and prediction leaderboard
- Odds history chart and champion celebration
- Offline PWA caching and 192px / 512px install icons
- Responsive layout for phones, tablets and desktop browsers

## Data and collaboration
By default, tournament data is stored in the browser's local storage on the current device. This version does not synchronize tournament entries or picks across different devices or users. The original optional hosted database integration remains in the app for environments that provide the expected `claude.use("user")` and `claude.use("db")` APIs.

## Deploy to GitHub Pages
1. Create a GitHub repository.
2. Upload the **contents** of this `esports-bracket-pwa` folder to the repository root (so `index.html` is at the root).
3. Open **Settings → Pages**.
4. Select **Deploy from a branch**, choose `main` and `/(root)`, then save.
5. Wait for GitHub Pages to publish the site.

All app assets use relative paths, so the app works from a GitHub Pages project subpath as well as a custom domain.

## Run locally
Use a local web server (for example VS Code Live Server) and open the served address. PWA installation and service-worker caching require HTTPS or localhost; opening `index.html` directly with `file://` will not enable those features.

## Install
- **Android:** Open the published HTTPS site in Chrome → menu → Install app / Add to Home screen.
- **Desktop:** Open the site in Chrome or Edge → use the install icon in the address bar or browser menu.

## Notes
The app honors the device's reduced-motion accessibility preference. The bracket scrolls horizontally on narrow screens; swipe sideways to move between rounds.
