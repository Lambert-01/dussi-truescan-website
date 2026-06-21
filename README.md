# DUSSI TrueScan Website

Static Astro website for DUSSI TrueScan KGL. Ltd.

## Local Development

```bash
npm install
npm run dev
```

Local URL:

```text
http://localhost:4321/
```

Admin control page:

```text
http://localhost:4321/admin
```

Admin password:

```text
truescan
```

## Build

```bash
npm run build
```

The static production output is generated in:

```text
dist/
```

## Vercel Deployment Settings

Vercel should auto-detect this as an Astro project.

Use these settings if Vercel asks:

```text
Framework Preset: Astro
Install Command: npm install
Build Command: npm run build
Output Directory: dist
Development Command: npm run dev
```

No backend, database, or server adapter is required for this project.

## Important Admin Note

The `/admin` page is a static, browser-based control panel. It saves changes in the browser using `localStorage` and can export/import JSON.

Because this site has no backend or database, `/admin` cannot permanently write changes to deployed Vercel files by itself. To make admin edits permanent, export JSON and update the source content before redeploying, or later connect a Git-based CMS.

## Deployment Flow

1. Push this project to GitHub.
2. Import the GitHub repository into Vercel.
3. Confirm Vercel uses the Astro preset.
4. Deploy.
5. Add your custom domain in Vercel Project Settings.

## Useful Commands

```bash
npm run dev
npm run build
npm run preview
```
