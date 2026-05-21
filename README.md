# Convert Master

Convert Master is a multi-tool web app built with Next.js. It provides free, browser-based utilities for image conversions/optimization and text transformations, plus a set of handy micro-tools.

Live site: https://tool-website-beta.vercel.app/

## Features

- Image tools: convert, optimize, and resize for popular platforms
- Text tools: repeat, reverse, bold/italic, and word count
- Utility tools: password generator, sudoku puzzle, and color picker
- Internationalization with English, German, and Hindi
- Analytics integrations (Vercel Analytics and Google Analytics)

## Tech Stack

- Next.js 14 (App Router), React 18, TypeScript
- MUI (Material UI), Emotion, Radix UI
- next-intl for localization
- Sharp, html2canvas, and other client utilities

## Getting Started

### Prerequisites

- Node.js 18+ recommended
- pnpm 10+ (used in this repo)

### Install

```bash
pnpm install
```

### Run locally

```bash
pnpm dev
```

Open http://localhost:3000 in your browser.

## Scripts

- `pnpm dev` - run the dev server
- `pnpm build` - build for production
- `pnpm start` - run the production server
- `pnpm lint` - run ESLint
- `pnpm format` - format the codebase with Prettier
- `pnpm format:check` - verify formatting

## Configuration

- Base URL is derived from `NODE_ENV` in [src/config/constants.ts](src/config/constants.ts)
- Supported locales are defined in [src/config.ts](src/config.ts)

## Project Structure

- [src/app](src/app) - App Router pages, routes, and layouts
- [src/components](src/components) - UI components and tool-specific widgets
- [messages](messages) - i18n message catalogs
- [public](public) - static assets, icons, and verification files

## Deployment

This project is optimized for Vercel. Build and deploy using:

```bash
pnpm build
pnpm start
```

## Contributing

Issues and PRs are welcome. Please keep changes focused and follow the existing code style.
