# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm init svelte

# create a new project in my-app
npm init svelte my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

```
my-app
├─ .gitignore
├─ .npmrc
├─ .svelte-kit
│  ├─ generated
│  │  ├─ client-manifest.js
│  │  ├─ client-matchers.js
│  │  └─ root.svelte
│  ├─ runtime
│  │  ├─ app
│  │  │  ├─ env.js
│  │  │  ├─ navigation.js
│  │  │  ├─ paths.js
│  │  │  └─ stores.js
│  │  ├─ client
│  │  │  ├─ singletons.js
│  │  │  └─ start.js
│  │  ├─ components
│  │  │  ├─ error.svelte
│  │  │  └─ layout.svelte
│  │  ├─ env.js
│  │  ├─ paths.js
│  │  └─ server
│  │     └─ index.js
│  ├─ tsconfig.json
│  └─ types
│     └─ src
│        └─ routes
│           ├─ __types
│           │  ├─ __layout-reset.d.ts
│           │  ├─ __layout.d.ts
│           │  └─ index.d.ts
│           └─ pages
│              ├─ __types
│              │  ├─ [link].d.ts
│              │  ├─ __layout@reset.d.ts
│              │  └─ index.d.ts
│              └─ post
│                 └─ __types
│                    ├─ [id].d.ts
│                    ├─ __layout@reset.d.ts
│                    └─ index.d.ts
├─ .vscode
│  └─ settings.json
├─ README.md
├─ folder-alias.json
├─ package-lock.json
├─ package.json
├─ src
│  ├─ app.html
│  ├─ lib
│  │  └─ title.svelte
│  └─ routes
│     ├─ __layout-reset.svelte
│     ├─ __layout.svelte
│     ├─ index.svelte
│     └─ pages
│        ├─ [link].svelte
│        ├─ __layout@reset.svelte
│        ├─ index.svelte
│        └─ post
│           ├─ [id].svelte
│           ├─ __layout@reset.svelte
│           └─ index.svelte
├─ static
│  └─ favicon.png
├─ svelte.config.js
└─ vite.config.js

```