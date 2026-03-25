# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Expense tracker app from Mosh's [Claude Code course](https://codewithmosh.com/p/claude-code). It intentionally has bugs, poor UI, and messy code — all fixed throughout the course.

## Commands

- `npm run dev` — Start Vite dev server (http://localhost:5173)
- `npm run build` — Production build
- `npm run lint` — ESLint

## Architecture

Single-component React 19 app with Vite 7. All state and UI live in `src/App.jsx` — no routing, no state library, no backend. Plain CSS styling via `App.css` and `index.css`.

## Known Intentional Issues

- Transaction amounts stored as strings, so `reduce()` concatenates instead of summing
- "Freelance Work" is typed as "expense" instead of "income"
