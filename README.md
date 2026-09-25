# EPANETLab.com

Marketing / landing site for [EPANETLab](https://epanetlab.com) — a browser-based
hydraulic modeling tool for water distribution networks. This site powers the
public homepage for [app.epanetlab.com](https://app.epanetlab.com).

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
  pages/index.astro    # homepage (hero, features, founder, FAQ)
  components/Icon.astro
  styles/global.css
public/
  favicon.svg          # EPANETLab app icon
  appicon.svg
  founder.png          # founder photo (About section)
  robots.txt
  sitemap.xml
```

## Theme

Dark, engineering/technical design with blueprint grid textures, monospace
accents, and a cyan "water" accent. Logo uses the water-gradient
`#4fc3f7 → #0277bd → #0d47a1`. SEO is baked in: canonical URL, Open Graph /
Twitter meta, JSON-LD `SoftwareApplication` structured data, `robots.txt` and
`sitemap.xml`.