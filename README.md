# SEB Italia - Secure. Ecological. Box.

![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=111111)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=ffffff)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=ffffff)
![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=ffffff)
![Supabase](https://img.shields.io/badge/Supabase-Lead%20Data-3FCF8E?style=for-the-badge&logo=supabase&logoColor=ffffff)
![Vercel](https://img.shields.io/badge/Vercel-Deploy-000000?style=for-the-badge&logo=vercel&logoColor=ffffff)

SEB Italia needed a launch-ready digital presence for a smart container product built around secure access, reusable materials, and urban logistics.
The result is a responsive React website that turns the product story into clear use cases, SEO-ready pages, and a Supabase-backed contact funnel.

## Preview

[![SEB Italia home page preview](output/playwright/sebitalia-home-hero.png)](https://sebitalia.com)

**Live website:** https://sebitalia.com

## Project Context

| Area | Details |
| --- | --- |
| Project | SEB Italia - Secure. Ecological. Box. |
| Client / sector | Official JODA product, distributed by SHORENMAR, within the DHEVYL GROUP ecosystem. Sector: smart containers, sustainable packaging, property access, events, and urban logistics. |
| Core problem | The product needed a credible web presence that could explain a new physical/digital logistics concept, make its benefits understandable, and collect qualified interest. |
| Delivered result | A public product website with bilingual content, product pages, use-case pages, structured SEO metadata, analytics hooks, and a working lead capture flow. |

## Tech Stack

| Layer | Implementation |
| --- | --- |
| Frontend | ![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=111111) ![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=ffffff) ![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=ffffff) |
| Styling | ![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-3-06B6D4?logo=tailwindcss&logoColor=ffffff) ![PostCSS](https://img.shields.io/badge/PostCSS-8-DD3A0A?logo=postcss&logoColor=ffffff) |
| Routing and UX | ![React Router](https://img.shields.io/badge/React%20Router-7-CA4245?logo=reactrouter&logoColor=ffffff) ![Lucide](https://img.shields.io/badge/Lucide-Icons-F56565?logo=lucide&logoColor=ffffff) |
| SEO and analytics | ![React Helmet](https://img.shields.io/badge/Helmet-SEO-222222) ![Vercel Analytics](https://img.shields.io/badge/Vercel%20Analytics-Enabled-000000?logo=vercel&logoColor=ffffff) |
| Data capture | ![Supabase](https://img.shields.io/badge/Supabase-Contacts-3FCF8E?logo=supabase&logoColor=ffffff) |
| Deployment | ![Vercel](https://img.shields.io/badge/Vercel-SPA%20Routing-000000?logo=vercel&logoColor=ffffff) |

## Features

- Product-led home page with a rotating hero, direct CTAs, and visual positioning around Secure, Ecological, and Box.
- Dedicated product and use-case pages covering smart lock, GPS tracking, NFC/QR access, technical specifications, property management, events, logistics, and rental/handling markets.
- Bilingual IT/EN content managed through a lightweight language context and translation files.
- Contact form connected to Supabase, with success/error states and direct email CTAs for demos, brochures, and pilot program requests.
- SEO foundation with sitemap, robots file, web manifest, JSON-LD structured data, route metadata, and Vercel analytics/speed insights.

## Architecture

The app is a Vite single-page application. `src/App.tsx` owns the route map and global layout, while `src/pages` contains the main public screens: home, products, applications, contact, legal pages, and admin views.

Reusable UI is split between `src/components/layout`, `src/components/sections`, `src/components/common`, and `src/components/ui`. Product content and reusable domain data live in `src/data`; translations are centralized in `src/translations` and exposed through `src/context/LanguageContext.tsx`.

External integration is intentionally narrow: `src/lib/supabase.ts` creates the Supabase client used by the contact flow, `src/utils/seo-config.ts` centralizes metadata/structured data, and `vercel.json` rewrites deep links back to the SPA entry point.

## Local Development

```bash
npm install
npm run dev
```

```bash
npm run build
npm run lint
npm run preview
```

## Results and Impact

- Shipped a live product website at https://sebitalia.com with clear navigation for product discovery and lead conversion.
- Converted a complex product concept into sector-specific pages for property managers, event operators, logistics teams, corporate services, and emerging rental/handling markets.
- Surfaced the product's measurable value propositions directly in the UI: 70% packaging reduction, 85% security increase, and 40% logistics efficiency improvement.
- Added operational trust signals through structured data, sitemap coverage, legal pages, cookie consent, analytics, speed insights, and a production-friendly Vercel routing setup.

## Contacts

- Website: https://sebitalia.com
- Email: info@sebitalia.com
- Instagram: https://www.instagram.com/seb_italia/
- Portfolio / group profile: https://dhevylgroup.com
