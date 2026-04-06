# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal website for pedroburon.info — a freelance software engineering services site. Built with Astro + Tailwind CSS v4, deployed to GitHub Pages. Content is in Spanish.

## Commands

- `npm run dev` — start dev server (localhost:4321)
- `npm run build` — build static site to `dist/`
- `npm run preview` — preview production build locally

## Architecture

- **Astro 6** static site, single-page for now
- **Tailwind CSS v4** via Vite plugin (no tailwind.config — uses CSS `@theme` in `src/styles/global.css`)
- Layout in `src/layouts/Layout.astro`, pages in `src/pages/`
- Design system: dark background (#0a0a0a), cyan accent (#22d3ee), monospace+sans font pairing (JetBrains Mono + Inter)
- Deploy: GitHub Actions workflow in `.github/workflows/deploy.yml` → GitHub Pages

## Key Decisions

- `site` is set to `https://www.pedroburon.info` in `astro.config.mjs`
- Contact email: ``hi@pedroburon.info``
- All copy is in Spanish
