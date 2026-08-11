# RenewGuard Landing Page

> **Note:** currently configured to deploy as `renewguard-landing-dev` on the free `*.workers.dev` subdomain, separate from any existing production deployment.

AntSolutions marketing site (static HTML/CSS/JS), split out from the main
RenewGuard monorepo for independent deployment.

Originally served by the Ktor backend at `/`; now deployed standalone.

## Deploy (Cloudflare Workers static assets)

```bash
npm install
npm run deploy
```

Point your DNS/custom domain (e.g. `renewguard.antsolutions.uk`) at this
Worker in the Cloudflare dashboard, or add a `routes` entry to
`wrangler.jsonc`.
