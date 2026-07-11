# NorthStar Home Performance — Website

This is a real, deployable React project (built with Vite). See the main
conversation for full step-by-step deployment instructions.

## Quick reference

- `npm install` then `npm run dev` to preview locally
- `npm run build` produces a `dist/` folder of static files
- Deploy by connecting this project to Vercel (recommended) — Vercel
  auto-detects Vite and builds it for you, no manual build step needed

## Important note on "Edit Site"

The in-page "Edit Site" panel originally saved content to Claude's built-in
storage. That doesn't exist outside Claude, so this package includes a
stand-in that saves to each visitor's own browser instead (via
localStorage). That means:

- It works — you can click Edit Site and it won't error
- But edits only show up in the browser that made them, not for other
  visitors, and not permanently across devices

For real content changes once this is live, the simplest path is asking
Claude to update the source and redeploying, rather than relying on the
live Edit Site panel.
