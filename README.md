# Today’s Bible Verse Website

The web project for Today’s Bible Verse, built with [Astro](https://astro.build).

The website is currently in its initial development stage. Its structure, navigation, dark color scheme, and public asset folders are established. Page content and final UI will be added incrementally.

## Current Pages

| Route | Purpose |
| --- | --- |
| `/` | Homepage |
| `/privacy/` | Privacy policy |
| `/404.html` | Page-not-found response |

## Project Structure

```text
/
├── public/
│   ├── images/
│   │   ├── app-screenshots/
│   │   └── logo.png
│   ├── store-badges/
│   ├── favicon.ico
│   └── favicon.svg
│
├── src/
│   ├── components/
│   │   ├── AppPromotion.astro
│   │   ├── ContactSection.astro
│   │   ├── DailyVerse.astro
│   │   ├── Footer.astro
│   │   └── Header.astro
│   │
│   ├── data/
│   │   └── verses.ts
│   │
│   ├── layouts/
│   │   └── BaseLayout.astro
│   │
│   ├── pages/
│   │   ├── 404.astro
│   │   ├── index.astro
│   │   └── privacy.astro
│   │
│   ├── scripts/
│   │   └── dailyVerse.ts
│   │
│   └── styles/
│       ├── global.css
│       └── variables.css
│
├── astro.config.mjs
├── package.json
├── package-lock.json
└── tsconfig.json
```

## Local Development

Install the project dependencies:

```sh
npm install
```

Start the local development server:

```sh
npm run dev
```

Astro will display the local website address, normally:

```text
http://localhost:4321
```

## Available Commands

| Command | Action |
| --- | --- |
| `npm install` | Installs project dependencies |
| `npm run dev` | Starts the local development server |
| `npm run build` | Creates the production website in `dist/` |
| `npm run preview` | Previews the production build locally |
| `npm run astro -- --help` | Displays Astro command help |

## Production Build

Create the static production website:

```sh
npm run build
```

The generated files are placed in:

```text
dist/
```

The `dist` directory is generated automatically and should not be edited manually.

## Deployment

The website is intended to be deployed as a static Astro site through Cloudflare.

Recommended Cloudflare build settings:

```text
Build command: npm run build
Build output directory: dist
```

## Content and Assets

- Place the primary website logo at `public/images/logo.png`.
- Place app screenshots in `public/images/app-screenshots/`.
- Place official app-store badges in `public/store-badges/`.
- Store the daily verse collection in `src/data/verses.ts`.
- Add shared colors and design values to `src/styles/variables.css`.
- Add site-wide styling to `src/styles/global.css`.

Empty asset directories contain `.gitkeep` files so Git can preserve them. These placeholders can be removed after real assets are added.

## Technology

- Astro
- TypeScript
- Static HTML and CSS
- Dark color scheme only