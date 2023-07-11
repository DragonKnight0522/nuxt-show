# NTN Boilerplate for Nuxt, Tailwind & NetlifyCMS

An easy-to-use starter kit with Nuxt.js, Vue 2, and Tailwindcss for launching a site on Netlify in minutes.

## Features

- **Nuxt.js** (SSR support)
- **Vue 2**
- **Tailwindcss** with PurgeCSS
- **Netlify CMS** (no server required)
- **PWA** support
- Responsive **dark mode**
- Pre-configured **Prettier** for code formatting

## Quickstart

1. Click the **Deploy to Netlify** button to create your site:
   
   [![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Knogobert/ntn-boilerplate&stack=cms)

2. After deploying, invite yourself as a user from **Netlify Identity**.
3. Set up a new password through the invite email.

## Local Development

- Install dependencies: `npm install`
- Start local dev server: `npm run dev`
- Build SSR deployment: `npm run build` then `npm run start`
- Generate a static site: `npm run generate`

## Personalization

1. Rename `.env-example` to `.env` and update the values.
2. Update metadata in `static/admin/config.yml`, `content/site/info.json`, and `package.json`.
3. Customize styles in `assets/scss/_vars.scss` & `tailwind.config.js`.
4. Change default font in `nuxt.config.js` and `tailwind.config.js`.

## Troubleshooting

If you face issues like CSS not appearing, inability to log into admin, or email login problems, check:

- Whitelisting classes in PurgeCSS (`nuxt.config.js`)
- Running `npx netlify-cms-proxy-server` for local CMS login
- Confirming Netlify Identity and Git Gateway setup
- Reviewing email template paths under Netlify Site Settings > Identity > Emails

Remember to set Netlify's `GIT_LFS_ENABLED` env variable to `true` for LFS support.