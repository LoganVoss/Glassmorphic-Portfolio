# Glassmorphic Portfolio

This is a simple next.js portfolio theme. It's open source for a reason! Use it ;D

Built with Next.js 16, React 19, TypeScript, Tailwind CSS 4, and Framer Motion.

## Run locally

Use Node.js 20.9 or later and npm. The included workflows use Node.js 20.

```bash
git clone https://github.com/LoganVoss/Glassmorphic-Portfolio.git
cd Glassmorphic-Portfolio
npm ci
npm run dev
```

Open [localhost:3000](http://localhost:3000) in your browser. Stop the development server with Ctrl+C.

## Make it yours

- [app/page.tsx](app/page.tsx): name, social links, experience, portfolio cards, and animation behavior.
- [app/globals.css](app/globals.css): glassmorphic styling and global CSS.
- [app/layout.tsx](app/layout.tsx): page title, description, font, and shared layout.
- [public/](public/): static assets.

Replace the included personal details and links before publishing your own version.

## Checks and builds

```bash
npm run lint
npm run build
```

These commands run ESLint and the Next.js production build, respectively. No automated test script is currently defined in [package.json](package.json).

## Deployment notes

The repository includes two [GitHub Pages workflows](.github/workflows/), both configured to run on pushes to `main`. They expect a static export in `out/`.

[next.config.mjs](next.config.mjs) declares `output: 'export'`; [next.config.ts](next.config.ts) also exists with an empty configuration. Review the configuration and workflow you intend to use before deploying. This README does not establish that deployment is currently passing.
