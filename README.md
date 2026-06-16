# Rustem Aisariyev — Portfolio (CS601 Term Project)

A personal portfolio site built with **React + TypeScript + Vite** and routed
with **React Router**. Nine content pages: Home, About, Interests, Resume,
Projects, Skills, Geolocation, Guestbook, and Contact.

Github pages link: https://rustem-stilinski.github.io/portfolio-2026/#/

---

## Run it locally

You need [Node.js](https://nodejs.org) 18+ installed.

```bash
npm install      # install dependencies
npm run dev      # start the dev server (http://localhost:5173)
npm run build    # type-check + production build into /dist
npm run preview  # preview the production build locally
npm run lint     # run ESLint
```



```

## Deploy to GitHub Pages (free hosting)

This project is already configured for Pages: `vite.config.ts` uses a relative
`base` and the app uses `HashRouter`, so links work with no server config.

```bash
npm run deploy
```

---

## Project structure

```
src/
├── components/    Navbar, Footer, ProjectCard, SkillBar, ThemeToggle,
│                  DecisionGraph, GalleryArt,
│                  GeoLocator
├── pages/         Home, About, Interests, Resume, Projects, Skills,
│                  Geolocation, Guestbook, Contact
├── context/       ThemeContext (light/dark, persisted)
├── hooks/         useTheme (custom hook)
├── services/      guestbook (CRUD: Supabase REST or localStorage)
├── data/          projects, skills, content (typed data modules)
├── types/         shared TypeScript interfaces
├── App.tsx        routes + layout
└── main.tsx       entry: HashRouter + ThemeProvider
```
