# It's Ridiculous — Frontend

The frontend for [It's Ridiculous API](https://github.com/MichalZak17/Its-Ridiculous-API). A collection of 120 absurd homework excuses, rated by absurdity, with predicted teacher reactions.

## Tech Stack

- **Astro** — Static site generation, zero client-side JS by default
- **Tailwind CSS v4** — Utility-first styling
- **TypeScript** — Type safety

All 120 excuses are embedded at build time from a local JSON file. No runtime API calls. Instant page loads.

## Project Structure

```
src/
  components/
    CategoryCard.astro
    ExcuseCard.astro
    RandomExcuse.astro
  data/
    excuses.json
  layouts/
    Layout.astro
  pages/
    index.astro
    explore.astro
    categories.astro
    about.astro
  styles/
    global.css
```

## Pages

| Route         | Description                                      |
| :------------ | :----------------------------------------------- |
| `/`           | Hero, random excuse generator, category overview |
| `/explore`    | All excuses with category filters and pagination |
| `/categories` | 10 categories with descriptions                  |
| `/about`      | Tech stack, API reference, disclaimer            |

## Getting Started

```sh
npm install
npm run dev
```

## Commands

| Command           | Action                                       |
| :---------------- | :------------------------------------------- |
| `npm install`     | Install dependencies                         |
| `npm run dev`     | Start local dev server at `localhost:4321`    |
| `npm run build`   | Build production site to `./dist/`           |
| `npm run preview` | Preview the production build locally         |

## License

MIT
