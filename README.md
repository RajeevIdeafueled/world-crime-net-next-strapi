# World Crime Net — Next.js + Strapi

Figma-driven implementation of the World Crime Net homepage and long-form story detail template.

## Stack
- Next.js 15 (App Router)
- React 19
- Strapi 5
- TypeScript

## Local development

### Frontend
```bash
cd frontend
cp .env.example .env.local
npm install
npm run dev
```

### Strapi
```bash
cd cms
cp .env.example .env
npm install
npm run develop
```

## Vercel
Deploy the `frontend` folder as the Vercel project root and set `NEXT_PUBLIC_STRAPI_URL` to the hosted Strapi API URL. The frontend includes fallback content when Strapi is unavailable.

Strapi should run on a persistent Node.js host with a managed database; Vercel is used for the Next.js frontend.