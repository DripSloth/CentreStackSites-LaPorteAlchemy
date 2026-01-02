
# CentreStack – La Porte Alchemy Website

This project is a static website built with **Astro**, designed for fast load times and strong SEO.  
It is deployed on **Cloudflare Pages** and follows a simple local-first development workflow.

---

## Tech Stack
- Astro (static site generation)
- Node.js (LTS)
- npm
- Cloudflare Pages (hosting)

---

## Local Development

Install dependencies:
```bash
npm install
````

Start the local development server:

```bash
npm run dev
```

The site will be available at:

```
http://localhost:4321
```

---

## Build

To generate the production build:

```bash
npm run build
```

The static output is generated in the `dist/` directory.

---

## Deployment

**Deployment target:** Cloudflare Pages

* The site is deployed automatically via Git integration.
* Any push to the `main` branch triggers a new build and deploy.
* Build command:

  ```bash
  npm run build
  ```
* Build output directory:

  ```
  dist
  ```

Cloudflare handles:

* Global CDN
* HTTPS / TLS
* DNS (when the domain is on Cloudflare)

---

## Environment Variables

If required, environment variables should be defined in:

```
.env
```

Do **not** commit `.env` files.
Use `.env.example` to document required variables.

---

## Notes

* This is a **static Astro build** (no SSR).
* JavaScript is shipped only where explicitly enabled.
* Optimised for SEO, performance, and long-term maintainability.