# Sparrow Creative — Next.js Creative Agency Website

A premium, production-ready creative agency website built with **Next.js 16**, **React 19**, **Tailwind CSS 4**, and **Framer Motion**. Features a modern design system, smooth animations, and a complete set of pages for a full-service creative agency.

[![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwindcss)](https://tailwindcss.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript)](https://www.typescriptlang.org/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-12-0055FF?logo=framer)](https://www.framer.com/motion/)

---

## 🎯 Overview

Sparrow Creative is a fully-featured creative agency website showcasing:
- **12+ Pages**: Home, About, Services, Portfolio, Team, Careers, Pricing, Blog, Contact, FAQ, Privacy Policy, Terms & Conditions
- **6 Core Services**: Brand Identity, Web Design, UI/UX Design, Development, SEO & Marketing, Motion Graphics
- **Dynamic Content**: Portfolio projects, blog posts, team members, pricing plans, FAQ data
- **Rich Animations**: Scroll-triggered reveals, parallax effects, magnetic interactions, staggered animations, counters
- **Responsive Design**: Mobile-first approach with desktop and mobile navigation (mega menu)
- **Performance Optimized**: Next.js App Router, Server Components, optimized images, code splitting

---

## 🚀 Quick Start

### Prerequisites

- **Node.js** 20.x or later
- **npm** 10.x or later (or yarn/pnpm/bun)

### Installation

```bash
# Clone the repository
git clone https://github.com/girishlade111/sparrow-creative.git
cd sparrow-creative

# Install dependencies
npm install

# Start development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the website.

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with Turbopack |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |

---

## 📁 Project Structure

```
sparrow-creative/
├── public/                     # Static assets
│   └── images/                 # Image assets (team, portfolio, blog, gallery)
├── src/
│   ├── app/                    # Next.js App Router pages
│   │   ├── about/              # About page
│   │   ├── blog/               # Blog listing & individual posts
│   │   │   └── [slug]/         # Dynamic blog post route
│   │   ├── careers/            # Careers page
│   │   ├── contact/            # Contact page
│   │   ├── faq/                # FAQ page
│   │   ├── portfolio/          # Portfolio listing & project details
│   │   │   └── [slug]/         # Dynamic portfolio project route
│   │   ├── pricing/            # Pricing page
│   │   ├── privacy-policy/     # Privacy Policy page
│   │   ├── services/           # Services listing & service details
│   │   │   └── [slug]/         # Dynamic service route
│   │   ├── team/               # Team page
│   │   ├── terms-conditions/   # Terms & Conditions page
│   │   ├── globals.css         # Global styles & Tailwind imports
│   │   ├── layout.tsx          # Root layout with providers
│   │   ├── page.tsx            # Homepage
│   │   └── not-found.tsx       # 404 page
│   ├── components/
│   │   ├── animations/         # Reusable animation components
│   │   │   ├── Counter.tsx     # Animated number counter
│   │   │   ├── Magnetic.tsx    # Magnetic hover effect
│   │   │   ├── ParallaxImage.tsx # Parallax scroll effect
│   │   │   ├── Reveal.tsx      # Scroll-triggered reveal
│   │   │   ├── StaggerContainer.tsx # Staggered children animation
│   │   │   └── index.ts        # Barrel exports
│   │   ├── home/               # Homepage-specific sections
│   │   │   ├── Hero.tsx        # Hero section with video
│   │   │   ├── WhySparrow.tsx  # Value proposition
│   │   │   ├── VideoShowcase.tsx # Video portfolio showcase
│   │   │   ├── Features.tsx    # Feature highlights
│   │   │   ├── Process.tsx     # 4-step process
│   │   │   ├── CtaBanner.tsx   # Call-to-action banner
│   │   │   ├── Performance.tsx # Stats & metrics
│   │   │   ├── PricingSection.tsx # Pricing cards
│   │   │   ├── TeamSection.tsx # Team members
│   │   │   ├── Gallery.tsx     # Image gallery
│   │   │   ├── CareersCta.tsx  # Careers CTA
│   │   │   └── index.ts        # Barrel exports
│   │   ├── layout/             # Layout components
│   │   │   ├── DesktopNav.tsx  # Desktop navigation with mega menu
│   │   │   ├── MobileNav.tsx   # Mobile navigation drawer
│   │   │   ├── MegaMenu.tsx    # Expandable mega menu
│   │   │   ├── Footer.tsx      # Site footer
│   │   │   ├── PageTransition.tsx # Page transition wrapper
│   │   │   └── index.ts        # Barrel exports
│   │   └── ui/                 # Base UI components
│   │       ├── Button.tsx      # Button variants
│   │       ├── Card.tsx        # Card components
│   │       ├── Input.tsx       # Form inputs
│   │       ├── Badge.tsx       # Badge/tag component
│   │       ├── Container.tsx   # Responsive container
│   │       ├── Section.tsx     # Section wrapper
│   │       ├── Grid.tsx        # Responsive grid
│   │       ├── Icon.tsx        # Lucide icon wrapper
│   │       └── index.ts        # Barrel exports
│   ├── data/
│   │   └── index.ts            # Re-exports from lib/data
│   ├── hooks/
│   │   ├── useScrollPosition.ts # Scroll position hook
│   │   ├── useIntersectionObserver.ts # Intersection observer hook
│   │   └── index.ts            # Barrel exports
│   └── lib/
│       ├── data.ts             # All site content & configuration
│       └── utils.ts            # Utility functions (cn, formatters)
├── .gitignore                  # Git ignore rules
├── AGENTS.md                   # AI agent instructions
├── CLAUDE.md                   # Claude Code configuration
├── DESIGN.md                   # Design system documentation
├── eslint.config.mjs           # ESLint configuration
├── next.config.ts              # Next.js configuration
├── next-env.d.ts               # Next.js TypeScript declarations
├── package.json                # Dependencies & scripts
├── package-lock.json           # Lock file
├── postcss.config.mjs          # PostCSS configuration
├── tsconfig.json               # TypeScript configuration
└── README.md                   # This file
```

---

## 🎨 Design System

### Colors

| Role | Light | Dark | Usage |
|------|-------|------|-------|
| Primary | `#1a1a2e` | `#f5f5f5` | Headlines, primary actions |
| Secondary | `#16213e` | `#e0e0e0` | Subheadings, secondary actions |
| Accent | `#e94560` | `#e94560` | CTAs, highlights, links |
| Background | `#ffffff` | `#0f0f1a` | Page backgrounds |
| Surface | `#f8f9fa` | `#1a1a2e` | Cards, containers |
| Border | `#e0e0e0` | `#2a2a3e` | Dividers, input borders |
| Muted | `#6b7280` | `#9ca3af` | Secondary text, placeholders |

### Typography

- **Headings**: Inter (variable font) — weights 400–700
- **Body**: Inter — weights 400, 500, 600
- **Scale**: Fluid typography using `clamp()` for responsive scaling

| Element | Desktop | Mobile |
|---------|---------|--------|
| H1 | `clamp(3rem, 8vw, 5rem)` | `clamp(2.5rem, 10vw, 3.5rem)` |
| H2 | `clamp(2rem, 5vw, 3rem)` | `clamp(1.75rem, 8vw, 2.5rem)` |
| H3 | `1.5rem` | `1.25rem` |
| Body | `1rem` / `1.125rem` | `1rem` |
| Small | `0.875rem` | `0.875rem` |

### Spacing System

Base unit: **4px** (0.25rem)

| Token | Value | Usage |
|-------|-------|-------|
| `space-1` | 4px | Micro spacing |
| `space-2` | 8px | Tight spacing |
| `space-3` | 12px | Small gaps |
| `space-4` | 16px | Standard gap |
| `space-5` | 20px | Medium spacing |
| `space-6` | 24px | Section padding |
| `space-8` | 32px | Large spacing |
| `space-10` | 40px | Section margins |
| `space-12` | 48px | XL spacing |
| `space-16` | 64px | Page-level spacing |
| `space-20` | 80px | Hero spacing |
| `space-24` | 96px | Major sections |

### Border Radius

| Token | Value |
|-------|-------|
| `rounded-sm` | 4px |
| `rounded-md` | 8px |
| `rounded-lg` | 12px |
| `rounded-xl` | 16px |
| `rounded-2xl` | 24px |
| `rounded-full` | 9999px |

### Shadows

| Token | Value |
|-------|-------|
| `shadow-sm` | `0 1px 2px 0 rgb(0 0 0 / 0.05)` |
| `shadow-md` | `0 4px 6px -1px rgb(0 0 0 / 0.1)` |
| `shadow-lg` | `0 10px 15px -3px rgb(0 0 0 / 0.1)` |
| `shadow-xl` | `0 20px 25px -5px rgb(0 0 0 / 0.1)` |
| `shadow-glow` | `0 0 40px -10px rgb(233 69 96 / 0.4)` |

---

## 🧩 Key Components

### Animation Components

| Component | Description | Props |
|-----------|-------------|-------|
| `Reveal` | Scroll-triggered fade/slide animations | `direction`, `delay`, `duration`, `once` |
| `StaggerContainer` | Staggered children animations | `stagger`, `delay`, `children` |
| `ParallaxImage` | Parallax scroll effect on images | `src`, `alt`, `speed`, `className` |
| `Magnetic` | Magnetic hover attraction | `strength`, `children` |
| `Counter` | Animated number counting | `end`, `duration`, `prefix`, `suffix` |

### Layout Components

| Component | Description |
|-----------|-------------|
| `DesktopNav` | Full-width navigation with mega menu dropdowns |
| `MobileNav` | Slide-out mobile drawer navigation |
| `MegaMenu` | Multi-column dropdown with service categories |
| `Footer` | Site footer with links, newsletter, social |
| `PageTransition` | Framer Motion page transitions |

### Homepage Sections

| Component | Description |
|-----------|-------------|
| `Hero` | Full-screen hero with headline, CTA, video background |
| `WhySparrow` | 3-column value proposition cards |
| `VideoShowcase` | Portfolio video player with thumbnail grid |
| `Features` | 6 feature cards with icons |
| `Process` | 4-step process timeline |
| `CtaBanner` | Mid-page conversion banner |
| `Performance` | Animated stat counters |
| `PricingSection` | 3-tier pricing cards |
| `TeamSection` | Team member cards with hover effects |
| `Gallery` | Masonry-style image gallery |
| `CareersCta` | Careers call-to-action |

### UI Primitives

| Component | Variants |
|-----------|----------|
| `Button` | `primary`, `secondary`, `outline`, `ghost`, `link` + sizes `sm`, `md`, `lg`, `xl` |
| `Card` | `default`, `hover`, `bordered` |
| `Input` | Text, email, textarea with label & error states |
| `Badge` | `default`, `outline`, `accent` |
| `Container` | Responsive max-width wrapper |
| `Section` | Vertical rhythm wrapper |
| `Grid` | Responsive CSS Grid layouts |

---

## 📄 Pages & Routes

| Route | Description | Dynamic |
|-------|-------------|---------|
| `/` | Homepage with all sections | No |
| `/about` | Agency story, mission, values | No |
| `/services` | 6-service grid overview | No |
| `/services/[slug]` | Individual service detail | Yes |
| `/portfolio` | Project showcase grid | No |
| `/portfolio/[slug]` | Project case study | Yes |
| `/team` | Team member profiles | No |
| `/careers` | Job openings & culture | No |
| `/pricing` | 3-tier pricing plans | No |
| `/blog` | Article listing with categories | No |
| `/blog/[slug]` | Individual blog post | Yes |
| `/contact` | Contact form & info | No |
| `/faq` | Accordion FAQ | No |
| `/privacy-policy` | Legal page | No |
| `/terms-conditions` | Legal page | No |

---

## 🔧 Configuration

### Next.js Config (`next.config.ts`)

```typescript
import type { NextConfig } from 'next'

const nextConfig: NextConfig = {
  reactStrictMode: true,
  images: {
    remotePatterns: [
      { protocol: 'https', hostname: '**' }
    ]
  },
  experimental: {
    optimizePackageImports: ['lucide-react', 'framer-motion']
  }
}

export default nextConfig
```

### TypeScript Config (`tsconfig.json`)

- **Target**: ES2017
- **Module**: ESNext
- **ModuleResolution**: Bundler
- **Strict**: true
- **Paths**: `@/*` → `./src/*`

### Tailwind CSS v4

- **Import**: `@import "tailwindcss"` in `globals.css`
- **Theme**: Custom design tokens in CSS variables
- **Dark Mode**: Class-based (`.dark`)

### ESLint Config

- **Extends**: `next/core-web-vitals`
- **Rules**: TypeScript-aware, React hooks, accessibility

---

## 🌐 Deployment

### Vercel (Recommended)

1. Push to GitHub
2. Import project in [Vercel](https://vercel.com/new)
3. Deploy — zero configuration needed

```bash
# Or deploy via CLI
npx vercel --prod
```

### Docker

```dockerfile
FROM node:20-alpine AS base
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:20-alpine AS runner
WORKDIR /app
ENV NODE_ENV=production
COPY --from=base /app/public ./public
COPY --from=base /app/.next/standalone ./
COPY --from=base /app/.next/static ./.next/static
EXPOSE 3000
CMD ["node", "server.js"]
```

Add to `next.config.ts`:
```typescript
const nextConfig: NextConfig = {
  output: 'standalone',
  // ...
}
```

### Static Export

For static hosting (Netlify, Cloudflare Pages, GitHub Pages):

```typescript
// next.config.ts
const nextConfig: NextConfig = {
  output: 'export',
  images: { unoptimized: true },
  // ...
}
```

```bash
npm run build
# Output in ./out/
```

---

## 🔒 Environment Variables

Create `.env.local` for local development:

```env
# Site configuration
NEXT_PUBLIC_SITE_URL=https://sparrowcreative.com
NEXT_PUBLIC_SITE_NAME="Sparrow Creative"

# Analytics (optional)
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX
NEXT_PUBLIC_VERCEL_ANALYTICS_ID=xxxx

# Forms (optional - for contact form)
CONTACT_FORM_ENDPOINT=https://api.example.com/contact
RECAPTCHA_SECRET_KEY=xxxx
```

---

## ♿ Accessibility

- **WCAG 2.2 AA** compliant
- Semantic HTML5 structure
- ARIA labels & roles on interactive elements
- Focus-visible outlines
- Keyboard navigation support
- Reduced motion support (`prefers-reduced-motion`)
- Color contrast ratios ≥ 4.5:1
- Alt text on all images
- Form labels & error associations

---

## ⚡ Performance

### Core Web Vitals Targets

| Metric | Target | Strategy |
|--------|--------|----------|
| LCP | < 2.5s | Optimized hero images, preload fonts |
| INP | < 200ms | Code splitting, minimal main thread work |
| CLS | < 0.1 | Explicit image dimensions, font display swap |

### Optimizations

- **Next.js App Router** — Server Components by default
- **Font Optimization** — `next/font` with `display: swap`
- **Image Optimization** — `next/image` with WebP/AVIF
- **Script Loading** — Deferred non-critical scripts
- **Bundle Analysis** — `npm run build && npx @next/bundle-analyzer`

---

## 🧪 Testing

```bash
# Unit & integration tests (when added)
npm run test

# E2E tests (when added)
npm run test:e2e

# Type checking
npm run lint
npx tsc --noEmit
```

---

## 📦 Dependencies

### Production

| Package | Version | Purpose |
|---------|---------|---------|
| `next` | 16.2.9 | React framework |
| `react` | 19.2.4 | UI library |
| `react-dom` | 19.2.4 | DOM renderer |
| `framer-motion` | 12.42.0 | Animations |
| `lucide-react` | 1.22.0 | Icons |
| `clsx` | 2.1.1 | Conditional classes |
| `tailwind-merge` | 3.6.0 | Tailwind class merging |
| `class-variance-authority` | 0.7.1 | Component variants |

### Development

| Package | Version | Purpose |
|---------|---------|---------|
| `typescript` | 5.x | Type checking |
| `eslint` | 9.x | Linting |
| `eslint-config-next` | 16.2.9 | Next.js ESLint config |
| `tailwindcss` | 4.x | CSS framework |
| `@tailwindcss/postcss` | 4.x | PostCSS plugin |
| `@types/node` | 20.x | Node types |
| `@types/react` | 19.x | React types |
| `@types/react-dom` | 19.x | React DOM types |

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

### Code Style

- Follow TypeScript strict mode
- Use functional components with hooks
- Prefer Server Components over Client Components
- Write meaningful commit messages (Conventional Commits)
- Run `npm run lint` before pushing

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

## 🙏 Acknowledgments

- **Next.js Team** — For the amazing framework
- **Vercel** — For hosting & developer experience
- **Tailwind CSS** — For the utility-first CSS framework
- **Framer Motion** — For production-ready animations
- **Lucide** — For beautiful, consistent icons
- **Unsplash** — For placeholder photography (replace with real images)

---

## 📞 Support

- **Email**: hello@sparrowcreative.com
- **Website**: [sparrowcreative.com](https://sparrowcreative.com)
- **Issues**: [GitHub Issues](https://github.com/girishlade111/sparrow-creative/issues)

---

**Built with ❤️ by the Sparrow Creative team**
## About the Author

**Built by Girish Lade** — [ladestack.in](https://ladestack.in)
