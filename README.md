
# Arianexa Presale Site Pack

This pack contains a responsive one-page presale site with Arianexa branding. You can:
- Host it as a static site (any host)
- Paste parts into **Framer**, **Typedream**, or **Webflow**
- Replace the iframe placeholder with your **presale widget** (Pinksale/Gempad/custom)

## Files
- `index.html` — landing page
- `styles.css` — styling (blue/black/white)
- `script.js` — countdown + placeholder logic
- `assets/` — images (logo, banner, tokenomics, roadmap)

## Quick Preview (Static Hosting)
1. Upload the whole folder to any static host (Vercel, Netlify, Cloudflare Pages, S3).
2. Open `/index.html`. Countdown is based on UTC: **2025-08-08T21:00:00Z**.

---

## Use in **Framer**
1. Create a new Framer project (dark theme recommended).
2. Add a **Code Component**:
   - Create a new code file and paste the snippet from `framer/CodeComponent.jsx` (included).
   - Import Google Fonts in the project settings > Fonts (`Fira Mono`, `Fauna One`).
3. Drag the `ArianexaLanding` component into the canvas and set to **Fill**.
4. Replace the **iframe** in the code with your presale widget embed (Pinksale/Gempad/custom dApp).
5. Upload images from `/assets/` to the Framer assets panel and update paths if needed.
6. Publish.

## Use in **Typedream**
1. Create a new page.
2. Add sections in order: Hero, Presale, Tokenomics, Roadmap, Community, Docs.
3. Use **Embed** blocks:
   - For the countdown + CTA, embed the html from `<section class="hero">...</section>`.
   - For the widget, add an **Embed** block and paste your Pinksale/Gempad code.
4. Upload `/assets/` images to Typedream and replace `src` paths in your embeds.
5. Apply background color `#05060A` and set fonts to *Fauna One* (body) and *Fira Mono* (code/mono).

## Use in **Webflow**
1. New project → Dark starter.
2. Create a page section structure matching the HTML.
3. For custom pieces (countdown/widget), add an **Embed** component and paste the respective HTML/JS from `index.html` and `script.js`.
4. Upload assets (logo/banner/tokenomics/roadmap) via the Webflow Assets panel.
5. Add Google Fonts `Fira Mono` and `Fauna One` via Project Settings → Fonts.
6. Publish to Webflow domain. (If using Webflow hosting, you don’t need `index.html`; recreate visually and copy code into Embeds.)

---

## Presale Widget Integration (Examples)
- **Pinksale**: Replace the placeholder `<iframe>` with the Pinksale sale page embed code from your launchpad dashboard.
- **Gempad**: Same approach—use the provided iframe/embed.
- **Custom dApp**: Remove the iframe and implement your Web3 logic; use `window.AX_CONFIG.CONTRACT_ADDRESS` and `CHAIN` for parameters.

## Countdown Timezone
The countdown uses **UTC** (`2025-08-08T21:00:00Z`). 10:00 PM WAT = 9:00 PM UTC.

## Contract & Links
- Network: **Base**
- Contract: **0xC1C3954ad740353a5F09c31a4aEc6bD4c34e2Ad1**
- Whitepaper: https://arianexa.xyz/Arianexa_Whitepaper.pdf
- X: https://x.com/Arianexa_ai
- Telegram: https://t.me/+Y8z9vseHZGM1NmU8
- Discord: https://discord.gg/ucK2Bx8xWT

---

## Notes
- Replace placeholder text/images as needed.
- Always test on **Base testnet** before mainnet.
