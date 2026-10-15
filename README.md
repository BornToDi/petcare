# PetCare / PetMAX Animal Care

Responsive veterinary clinic website built with React, TypeScript, TanStack Start, Vite, and Tailwind CSS.

Includes a redesigned landing page, local image assets, services, team, clinic gallery, contact information, responsive navigation, scroll reveal animations, reading progress, and a back-to-top control. Animations respect reduced-motion preferences.

## Run locally

Use Node.js 22.13+ or Node.js 24.

```sh
npm ci --legacy-peer-deps
npm run dev -- --host 127.0.0.1 --port 5173
```

Open http://127.0.0.1:5173/.

On Windows PowerShell, use `npm.cmd` if script execution policy blocks `npm`.

## Validation and limitations

```sh
npx tsc --noEmit
```

Desktop, tablet, and mobile navigation and bidirectional scroll animations were verified in Chrome. All images used by the landing page resolve locally.

The current production build needs Vite/TanStack version alignment: `npm run build` currently fails with an unresolved `index.html` entry. The development server works. The appointment form is presentational and does not submit bookings to a backend.
