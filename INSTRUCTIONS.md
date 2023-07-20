# Environment Setup

npx create-next-app@latest ai-saas --typescript --tailwind --eslint
√ Would you like to use `src/` directory with this project? ... No
√ Use App Router (recommended)? ... Yes
√ Would you like to customize the default import alias? ... No

cd ai-saas

npx shadcn-ui@latest init
√ Which style would you like to use? » Default
√ Which color would you like to use as base color? » Slate
√ Where is your global CSS file? ... app/globals.css
√ Do you want to use CSS variables for colors? ... yes
√ Where is your tailwind.config.js located? ... tailwind.config.js
√ Configure the import alias for components: ... @/components
√ Configure the import alias for utils: ... @/lib/utils
√ Are you using React Server Components? ... yes
√ Write configuration to components.json. Proceed? ... yes

- npm run dev

npm i @trivago/prettier-plugin-sort-imports

npx shadcn-ui@latest add button

# Folder Setup

...

# Clerk Authentication

www.clerk.com
Sign in for free account
Dashboard - Add application
Application name: ai-saas

- Provider: Google, Email
- Create application
- copy environment variables
- add to .env
- Continue in docs

npm install @clerk/nextjs

add to .env
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

.change app name in clerk dashboard
www.clerk.com - dashboard

- customization - branding
- application name: "Genius" - apply changes
