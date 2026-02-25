# Astro shadcn/ui template

A modern starter template using [Astro](https://astro.build/), [Tailwind CSS](https://tailwindcss.com/), and [shadcn/ui](https://ui.shadcn.com/) - perfect for building fast, accessible, and themeable web apps.

This template is configured to deploy to **Cloudflare Workers/Pages** for optimal performance at the edge.

---

## Getting Started

Before you begin, ensure that you have **Node.js** and **pnpm** (or **npm**) installed.

### Setup

```bash
git clone https://github.com/area44/astro-shadcn-ui-template
cd astro-shadcn-ui-template
pnpm install  # or npm install
pnpm dev      # or npm run dev
```

Open your browser and go to [http://localhost:4321](http://localhost:4321) to see the app running.

## Deployment

### Cloudflare Workers/Pages

This template is pre-configured for Cloudflare deployment with:

- `@astrojs/cloudflare` adapter for SSR support
- `wrangler.jsonc` configuration file
- Node.js compatibility enabled

#### Deploy to Cloudflare

1. **Build and deploy:**

   ```bash
   npm run deploy  # or pnpm deploy
   ```

2. **Test locally with Wrangler:**

   ```bash
   npm run cf:dev  # or pnpm cf:dev
   ```

3. **Deploy via Cloudflare Dashboard:**
   - Connect your GitHub repository to Cloudflare Pages
   - Build command: `npm run build`
   - Build output directory: `dist`

For more information, see the [Cloudflare Astro deployment guide](https://developers.cloudflare.com/pages/framework-guides/deploy-an-astro-site/).

## Adding Components

`shadcn/ui` provides pre-built, accessible UI components. To add one:

1. Follow the official [Astro installation guide](https://ui.shadcn.com/docs/installation/astro).
2. Pick a component (e.g., [Accordion](https://ui.shadcn.com/docs/components/accordion), [Dialog](https://ui.shadcn.com/docs/components/dialog)) and follow the usage instructions.

> [!NOTE]
> In Astro, an [island](https://docs.astro.build/en/concepts/islands/) is an interactive component rendered on the client. For complex or dynamic components, check [Add a Shadcn UI Component | Space Madness Stack](https://spacemadness.dev/docs/add-a-shadcn-ui-component)

If you're new to using React (or other frameworks) inside Astro, start with the [Framework Components guide](https://docs.astro.build/en/guides/framework-components/).

## License

This project is licensed under the [MIT License](LICENSE).
