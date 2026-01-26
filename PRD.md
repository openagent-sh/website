# OpenAgent Website - PRD

> Product Requirements Document for open-agent.sh

---

## Project Overview

| Key | Value |
|-----|-------|
| **Domain** | open-agent.sh |
| **Repository** | github.com/openagent-sh/website |
| **Main Repo** | github.com/openagent-sh/openagent |
| **Status** | Alpha |
| **Tagline** | "Your cofounder for life" |

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| **Astro 5.x** | Static site generator |
| **Tailwind CSS** | Styling (@astrojs/tailwind) |
| **Geist Mono** | Typography (local woff2 files) |
| **Lucide Icons** | Iconography |
| **Vercel** | Deployment |

---

## Design System

### Colors

```css
--background: #09090b;        /* Pure dark */
--text-primary: #fafafa;      /* Crisp white */
--text-muted: #a1a1aa;        /* Gray for secondary text */
--text-faded: #71717a;        /* Faded for subtle elements */
--border: rgba(255,255,255,0.1); /* Subtle borders */
--surface: #18181b;           /* Cards, elevated surfaces */
```

**Accent**: None - pure monochrome aesthetic

### Typography

| Element | Font | Weight | Size |
|---------|------|--------|------|
| Headlines | Geist Mono | SemiBold (600) | 48-72px |
| Subheadlines | Geist Mono | Medium (500) | 24-32px |
| Body | Geist Mono | Regular (400) | 16-18px |
| Small/Labels | Geist Mono | Regular (400) | 12-14px |

### Spacing

- Base unit: 4px
- Section padding: 80-120px vertical
- Content max-width: 1200px
- Card padding: 24-32px

### Animations

- **Level**: Minimal
- Hover states on buttons/links
- Smooth scroll for anchor links
- No scroll-triggered animations
- No particles or complex motion

### Grid Background

- Subtle grid pattern overlay
- Nearly invisible lines (~5% opacity)
- Grid size: ~60-80px squares

---

## Page Sections

### 1. Navigation

```
[Logo: OpenAgent]                    Features   Docs   [GitHub Button]
```

- **Position**: Sticky top
- **Style**: Transparent, blur on scroll optional
- **Logo**: Text-based "OpenAgent"
- **Links**: Features (anchor), Docs (→ GitHub README), GitHub (button)

### 2. Hero Section

```
                    [ Alpha ]
                    
        Your cofounder
           for life

   A personal AI operating system that remembers,
   adapts, and grows with you. Build faster.
   Think clearer. Ship more.

   [Get Started →]  [☆ Star on GitHub]

   ┌─────────────────────────────────────┐
   │  Terminal Mockup (hero.png)         │
   └─────────────────────────────────────┘
```

- **Badge**: "Alpha" - subtle, muted
- **Headline**: "Your cofounder" (white) + "for life" (faded gray)
- **Subtext**: Emotional + technical mix
- **CTAs**: 
  - Primary: "Get Started" (white bg, dark text)
  - Secondary: "Star on GitHub" (outline)
- **Visual**: Static terminal mockup using hero.png

### 3. Highlights Banner

```
Open Source  ·  Built on OpenCode  ·  Fast Onboarding  ·  Modular Configuration
```

- Single horizontal strip
- Muted text, subtle separator dots
- Links where appropriate (OpenCode → opencode.ai)

### 4. Problem / Solution

**Two-column layout:**

| THE PROBLEM | THE SOLUTION |
|-------------|--------------|
| **AI tools forget you the moment you close the tab** | **An AI that actually knows you** |
| Every conversation starts from zero. Your context, preferences, and history—gone. You're constantly re-explaining yourself to tools that should know you by now. | OpenAgent is your personal AI operating system. It remembers your projects, understands your preferences, and evolves alongside you. One system, infinite context. |

### 5. Features Grid

**6 Cards, 3x2 layout on desktop, 2x3 or 1x6 on mobile**

| Icon | Title | Description |
|------|-------|-------------|
| Brain | **Persistent Memory** | Your agent remembers everything—conversations, preferences, project context. No more starting from scratch. |
| GitBranch | **Autonomous Agents** | Deploy specialized agents that work in the background. Research, monitor, automate—all on your behalf. |
| Terminal | **Native CLI** | Full command-line interface for power users. Scriptable, composable, and blazingly fast. |
| Settings | **Simple Config** | One markdown file to rule them all. Version control your AI setup like any other codebase. |
| Puzzle | **Fully Extensible** | Build custom plugins and integrations. Connect to any API, database, or service you need. |
| User | **Deeply Personalized** | The more you use it, the better it gets. Your agent learns your style, priorities, and workflow. |

### 6. Use Cases

**3 Cards, horizontal layout**

| Icon | Title | Description |
|------|-------|-------------|
| Code | **Developers** | Ship faster with an AI that knows your codebase, your patterns, and your preferences. |
| Rocket | **Founders** | A cofounder who remembers every decision, every pivot, every lesson learned. |
| CheckSquare | **Personal** | Tasks, habits, goals—one system that grows with you and keeps you on track. |

### 7. Install Section

```
                    Get Started

   ┌──────────────────────────────────────────────┐
   │ git clone https://github.com/openagent-sh/  │
   │ openagent                                    │
   │ cd openagent                                 │
   │ ./setup.sh                                   │  [Copy]
   └──────────────────────────────────────────────┘
```

- Monospace code block
- Copy button (click to copy)
- Dark surface background

### 8. FAQ Section

**Accordion style - click to expand**

| Question | Answer |
|----------|--------|
| What is OpenAgent? | OpenAgent is a personal AI operating system that lives on your machine. It combines persistent memory, specialized agents, and deep personalization to create an AI that truly knows you. |
| Why OpenAgent? | Unlike ChatGPT or Claude, OpenAgent doesn't forget you. It builds context over time, understands your projects, and grows alongside your needs. It's your AI cofounder for life. |
| How do I get started? | Clone the repository, run the setup script, and complete the onboarding flow. In 5 minutes, OpenAgent will understand who you are and what you're building. |
| Where is my data stored? | Everything stays local on your machine. OpenAgent is local-first and privacy-respecting. Your data never leaves your computer unless you explicitly choose to sync it. |
| Is it free and open source? | Yes. OpenAgent is completely free and open source. Use it, modify it, contribute to it. |
| How can I contribute? | Check out our GitHub repository, read the contributing guide, and join the community. We welcome all contributions—code, docs, ideas. |

### 9. Footer

```
─────────────────────────────────────────────────────────────

OpenAgent — Your cofounder for life.

GitHub    Docs    Install

Made for developers who want more from AI.

@rvm0n_

─────────────────────────────────────────────────────────────
```

- Tagline repeat
- Key links: GitHub, Docs (→ README), Install (anchor)
- Social: X link (@rvm0n_)
- Subtle closing line

---

## SEO & Meta

```html
<title>OpenAgent - Your cofounder for life</title>
<meta name="description" content="A personal AI operating system that remembers, adapts, and grows with you. Open source, local-first, deeply personalized." />

<!-- Open Graph -->
<meta property="og:title" content="OpenAgent - Your cofounder for life" />
<meta property="og:description" content="A personal AI operating system that remembers, adapts, and grows with you." />
<meta property="og:image" content="/og-image.png" />
<meta property="og:url" content="https://open-agent.sh" />

<!-- Twitter -->
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:site" content="@rvm0n_" />
```

---

## Assets

### Required

- [x] `public/hero.png` - Terminal mockup (already present)
- [ ] `public/fonts/GeistMono-Regular.woff2`
- [ ] `public/fonts/GeistMono-Medium.woff2`
- [ ] `public/fonts/GeistMono-SemiBold.woff2`
- [ ] `public/og-image.png` - Open Graph image (1200x630)

### Source Fonts

Copy from: `/Users/ramon/Downloads/geist-font-1.6.0/fonts/GeistMono/webfonts/`

---

## Responsive Breakpoints

| Breakpoint | Width | Layout Changes |
|------------|-------|----------------|
| Mobile | < 640px | Single column, stacked sections |
| Tablet | 640-1024px | 2-column grids |
| Desktop | > 1024px | Full layout, 3-column features |

---

## Implementation Order

### Phase 1: Foundation
1. Install Tailwind (@astrojs/tailwind)
2. Copy Geist Mono fonts to /public/fonts/
3. Create base layout with font-face declarations
4. Set up color variables in Tailwind config
5. Create grid background pattern

### Phase 2: Components
1. Navigation component
2. Hero section with terminal mockup
3. Footer component
4. Button components (primary, outline)
5. Card component

### Phase 3: Sections
1. Highlights banner
2. Problem/Solution section
3. Features grid
4. Use Cases section
5. Install section with copy button
6. FAQ accordion

### Phase 4: Polish
1. Responsive adjustments
2. SEO meta tags
3. Favicon (keep Astro default for now)
4. Final review and testing
5. Deploy to Vercel

---

## Links & References

- **OpenCode**: https://opencode.ai
- **GitHub Org**: https://github.com/openagent-sh
- **Main Repo**: https://github.com/openagent-sh/openagent
- **Website Repo**: https://github.com/openagent-sh/website
- **X/Twitter**: https://x.com/rvm0n_

---

## Notes

- No analytics/tracking
- No testimonials or pricing
- No newsletter signup
- Favicon: Keep Astro default for now
- /docs route redirects to GitHub README

---

*Created: 2026-01-25*
