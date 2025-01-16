<a name="readme-top"></a>

# Freespace - A Collaborative Whiteboard Website using Next.js 14

<!-- Table of Contents
<details>
<summary>

# Table of Contents

</summary>

- [Folder Structure](#bangbang-folder-structure)
- [Getting Started](#toolbox-getting-started)
- [Screenshots](#camera-screenshots)
- [Tech Stack](#gear-tech-stack)
- [Acknowledgements](#gem-acknowledgements)
- [Deploy on Vercel](#page_with_curl-deploy-on-vercel)

</details> -->

## Folder Structure

Here is the folder structure of this app.

```bash
freespace/
  |- app/
    |-- _components/
        |--- AdBanner.tsx
        |--- Header.tsx
        |--- Hero.tsx
    |-- _constant/
        |--- Constant.tsx
    |-- _context/
        |--- FileListContext.tsx
    |-- (routes)/
        |--- dashboard/
            |---- _components/
                |----- FileList.tsx
                |----- Header.tsx
                |----- PricingDialog.tsx
                |----- SideNav.tsx
                |----- SideNavBottomSection.tsx
                |----- SideNavTopSection.tsx
            |---- layout.tsx
            |---- page.tsx
        |--- teams/
            |---- create/
                |----- page.tsx
        |--- workspace/
            |---- _components/
                |----- Canvas.tsx
                |----- Editor.tsx
                |----- WorkspaceHeader.tsx
            |---- [fileId]/
                |----- page.tsx
    |-- api/
        |--- auth/
            |---- [kindeAuth]/
                |----- route.js
    |-- ConvexClientProvider.tsx
    |-- favicon.ico
    |-- globals.css
    |-- layout.tsx
    |-- page.tsx
  |- components/
      |-- ui/
          |--- dialog.tsx
          |--- button.tsx
          |--- dropdown-menu.tsx
          |--- input.tsx
          |--- popover.tsx
          |--- separator.tsx
          |--- sonner.tsx
  |- convex/
      |-- _generated/
          |--- api.d.ts
          |--- api.js
          |--- dataModel.d.ts
          |--- server.d.ts
          |--- server.js
      |-- files.tsx
      |-- teams.tsx
      |-- user.tsx
  |- public/
      |-- create-team.png
      |-- landing-page.png
      |-- logo-1.png
      |-- logo-black.png
      |-- moder-uiux.png
      |-- next.svg
      |-- thoughts.png
      |-- vercel.svg
  |- .env.local
  |- .gitignore
  |- components.json
  |- middleware.ts
  |- next.config.mjs
  |- package-lock.json
  |- package.json
  |- postcss.config.js
  |- tailwind.config.ts
  |- tsconfig.json
```

<br />

## Getting Started

1. Make sure **Git** and **NodeJS** is installed.
2. Clone this repository to your local computer.
3. Create `.env.local` file in root directory.
4. Contents of `.env.local`:

```bash
# .env.local

# kinde credentials
KINDE_CLIENT_ID=<your-kinde-client-id>
KINDE_CLIENT_SECRET=<your-kinde-client-secret>
KINDE_ISSUER_URL=<your-kinde-url>
KINDE_SITE_URL=http://localhost:3000
KINDE_POST_LOGOUT_REDIRECT_URL=http://localhost:3000
KINDE_POST_LOGIN_REDIRECT_URL=http://localhost:3000/dashboard

# Deployment used by `npx convex dev`
CONVEX_DEPLOYMENT=dev:xxxxxxxxxxxx # team: ayan-maity, project: write-xxxxxx

NEXT_PUBLIC_CONVEX_URL=<your-next-convex-url>

```

11. Open terminal in root directory. Run `npm install` or `yarn install`.

12. Now app is fully configured 👍 and you can start using this app using `npm run dev` or `yarn dev`.

## Screenshots:

![Landing Page](/public/landing-page.png "Landing Page")

![Modern UI/UX](/public/moder-uiux.png "Modern UI/UX")

![Create Team](/public/create-team.png "Create Team")

![Express Your Thoughts](/public/thoughts.png "Express Your Thoughts")

## Tech Stack

[![React JS](https://skillicons.dev/icons?i=react "React JS")](https://react.dev/ "React JS") [![Next JS](https://skillicons.dev/icons?i=next "Next JS")](https://nextjs.org/ "Next JS") [![Typescript](https://skillicons.dev/icons?i=ts "Typescript")](https://www.typescriptlang.org/ "Typescript") [![Tailwind CSS](https://skillicons.dev/icons?i=tailwind "Tailwind CSS")](https://tailwindcss.com/ "Tailwind CSS") [![Vercel](https://skillicons.dev/icons?i=vercel "Vercel")](https://vercel.app/ "Vercel")

## Acknowledgements

Useful resources and dependencies that are used in FreeSpace.

- [@editorjs/checklist](https://www.npmjs.com/package/@editorjs/checklist) - Version: ^1.6.0
- [@editorjs/editorjs](https://www.npmjs.com/package/@editorjs/editorjs) - Version: ^2.29.0
- [@editorjs/header](https://www.npmjs.com/package/@editorjs/header) - Version: ^2.8.1
- [@editorjs/list](https://www.npmjs.com/package/@editorjs/list) - Version: ^1.9.0
- [@editorjs/paragraph](https://www.npmjs.com/package/@editorjs/paragraph) - Version: ^2.11.3
- [@editorjs/warning](https://www.npmjs.com/package/@editorjs/warning) - Version: ^1.4.0
- [@excalidraw/excalidraw](https://www.npmjs.com/package/@excalidraw/excalidraw) - Version: ^0.17.3
- [@kinde-oss/kinde-auth-nextjs](https://www.npmjs.com/package/@kinde-oss/kinde-auth-nextjs) - Version: ^2.1.13
- [@radix-ui/react-dialog](https://www.npmjs.com/package/@radix-ui/react-dialog) - Version: ^1.0.5
- [@radix-ui/react-dropdown-menu](https://www.npmjs.com/package/@radix-ui/react-dropdown-menu) - Version: ^2.0.6
- [@radix-ui/react-popover](https://www.npmjs.com/package/@radix-ui/react-popover) - Version: ^1.0.7
- [@radix-ui/react-separator](https://www.npmjs.com/package/@radix-ui/react-separator) - Version: ^1.0.3
- [@radix-ui/react-slot](https://www.npmjs.com/package/@radix-ui/react-slot) - Version: ^1.0.2
- [class-variance-authority](https://www.npmjs.com/package/class-variance-authority) - Version: ^0.7.0
- [clsx](https://www.npmjs.com/package/clsx) - Version: ^2.1.0
- [convex](https://www.npmjs.com/package/convex) - Version: ^1.9.1
- [lucide-react](https://www.npmjs.com/package/lucide-react) - Version: ^0.335.0
- [moment](https://www.npmjs.com/package/moment) - Version: ^2.30.1
- [next](https://www.npmjs.com/package/next) - Version: 14.1.0
- [next-themes](https://www.npmjs.com/package/next-themes) - Version: ^0.2.1
- [react](https://www.npmjs.com/package/react) - Version: ^18
- [react-dom](https://www.npmjs.com/package/react-dom) - Version: ^18
- [sonner](https://www.npmjs.com/package/sonner) - Version: ^1.4.0
- [tailwind-merge](https://www.npmjs.com/package/tailwind-merge) - Version: ^2.2.1
- [tailwindcss-animate](https://www.npmjs.com/package/tailwindcss-animate) - Version: ^1.0.7
- [@types/node](https://www.npmjs.com/package/@types/node) - Version: ^20
- [@types/react](https://www.npmjs.com/package/@types/react) - Version: ^18
- [@types/react-dom](https://www.npmjs.com/package/@types/react-dom) - Version: ^18
- [autoprefixer](https://www.npmjs.com/package/autoprefixer) - Version: ^10.0.1
- [postcss](https://www.npmjs.com/package/postcss) - Version: ^8
- [tailwindcss](https://www.npmjs.com/package/tailwindcss) - Version: ^3.3.0
- [typescript](https://www.npmjs.com/package/typescript) - Version: ^5

<!-- ## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details. -->
