# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for **Lar Arquitetura**, an architecture firm in Maringá/PR (Brazil) focused on real estate developers (incorporadoras). The site targets incorporadoras and investors seeking differentiated, identity-driven architecture.

## Commands

- `npm run dev` — start dev server (localhost:3000)
- `npm run build` — static export build
- `npx serve out` — serve the static export locally

## Tech Stack

Next.js 15 (App Router, static export) + Tailwind CSS v4 + Framer Motion + Lucide React

## Project Structure

- `src/app/` — layout.tsx (fonts, metadata, JSON-LD), page.tsx (assembles sections), globals.css (design tokens)
- `src/components/sections/` — 10 section components (hero, social-proof, why-us, services, process, testimonials, target-audience, cta, faq, footer)
- `src/components/ui/` — reusable primitives (FadeIn, StaggerContainer, SectionLabel)
- `src/components/layout/` — Header, MobileMenu
- `src/constants/` — content.ts (all PT-BR copy), animations.ts (Framer Motion variants), navigation.ts
- `src/hooks/` — useCountUp, useHeaderScroll, useReducedMotion

## Design System Essentials

- **Colors:** Primary #1A1A1A (dark), Accent #C9A96E (gold), Backgrounds alternate between #FFFFFF, #FAFAF7, #F5F3EF
- **Typography:** Playfair Display (headings, weight 400, italic for emphasis) + Inter (body)
- **Components:** All components use border-radius: 0px (rectangular aesthetic reflecting architecture)
- **Icons:** Lucide icons, line-style
- **Images:** Unsplash, architecture/minimal theme
- **Language:** PT-BR throughout

## Architecture (10 sections)

Hero → Social Proof (numbers) → Why Us (2x2 cards) → Services (alternating image/text) → Process (4 steps) → Testimonials (3 cards) → Target Audience (3 cards) → CTA (dark) → FAQ (accordion) → Footer (4-col dark)

## Key Constraints

- No border-radius anywhere — rectangular forms reinforce the architectural aesthetic
- Generous whitespace (section padding: clamp 5rem-10rem)
- Animations: subtle fade-in-up on scroll via Intersection Observer, count-up for statistics, staggered reveals
- Header: fixed, transparent → white on scroll with backdrop-blur
- Mobile: single column, hamburger with dark overlay, full-width buttons
