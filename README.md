# EPANETLab.com

Marketing / landing site for [EPANETLab](https://epanetlab.com) — a browser-based
hydraulic modeling tool for water distribution networks. This site powers the
public homepage with a launch countdown for [app.epanetlab.com](https://app.epanetlab.com).

Built with [Astro](https://astro.build). Static output, deployable on Vercel.

## Development

```sh
npm install
npm run dev      # start dev server
npm run build    # build static site into dist/
npm run preview  # preview the production build
```

## Deploy (Vercel)

- Framework preset: **Astro** (auto-detected)
- Build command: `npm run build`
- Output directory: `dist/`
- Site domains: `epanetlab.com` (production) + your Vercel preview URL

## Structure

```
src/
  pages/index.astro    # homepage (hero, countdown, features, FAQ)
  components/Icon.astro
  styles/global.css
public/
  favicon.svg          # EPANETLab app icon
  appicon.svg
```

The countdown anchors to `now + 10 days` on first visit and persists it in
`localStorage`, so every visitor counts down to the same launch instant.

## Theme

Colors and the droplet logo are pulled from the EPANETLab app (Vercel app
`epanetlab-two.vercel.app`, source in the `HydroNet` repo). Primary accent is
`#2563eb`; the logo uses the water-gradient `#4fc3f7 → #0277bd → #0d47a1`.