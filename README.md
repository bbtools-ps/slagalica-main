# Slagalica - Main Application

A modern web application that integrates two popular games from the Serbian quiz show "Slagalica" using a microfrontend architecture built with Astro.

## 🎮 About

This project serves as a central hub for two independently developed game applications:

- **Moj Broj** - A mathematical numbers game (React + Vite)
- **Slagalica** - A word puzzle game (Custom MVC + Parcel)

Both games are hosted separately on Netlify and integrated into this Astro application using iframe-based microfrontend architecture.

## 🏗️ Architecture

This application demonstrates a **microfrontend architecture** where:

- Each game is developed and deployed independently
- The main Astro app acts as a shell/host application
- Games are loaded at runtime via iframes
- Complete isolation between applications (styles, scripts, state)

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)
- pnpm

### Installation

```sh
pnpm install
```

### Development

```sh
pnpm dev
```

Starts local dev server at `localhost:4321`

### Build

```sh
pnpm build
```

Build your production site to `./dist/`

### Preview

```sh
pnpm preview
```

Preview your build locally before deploying

## 🔗 Integrated Applications

- **Moj Broj**: [https://bbtools-moj-broj.netlify.app/](https://bbtools-moj-broj.netlify.app/)
- **Slagalica**: [https://bbtools-slagalica.netlify.app/](https://bbtools-slagalica.netlify.app/)

## 🛠️ Technology Stack

- **Framework**: [Astro](https://astro.build)
- **Package Manager**: pnpm
- **Integration Pattern**: Iframe-based microfrontends
- **Deployment**: Netlify (for all applications)

## 📝 Key Features

- ✅ **Independent Deployments** - Each game can be updated without affecting others
- ✅ **Loading States** - Custom spinner component with smooth transitions
- ✅ **Reusable Components** - `MicrofrontendFrame` for easy integration of new apps
- ✅ **Type Safety** - TypeScript support throughout
- ✅ **Modern Build** - Optimized Astro builds for performance

## 🧞 Available Commands

| Command          | Action                                           |
| :--------------- | :----------------------------------------------- |
| `pnpm install`   | Installs dependencies                            |
| `pnpm dev`       | Starts local dev server at `localhost:4321`      |
| `pnpm build`     | Build your production site to `./dist/`          |
| `pnpm preview`   | Preview your build locally, before deploying     |
| `pnpm format`    | Format code with Prettier                        |
| `pnpm astro ...` | Run CLI commands like `astro add`, `astro check` |

## 📚 Learn More

- [Astro Documentation](https://docs.astro.build)
- [Microfrontend Architecture](https://micro-frontends.org/)

## 📄 License

This project is part of the BBTools collection.
