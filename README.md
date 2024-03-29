# todos-sveltekit

<img alt="todos svelte image" src="todosmvc-svelte.png" width="400" />

This is a simple [SvelteKit v2.0](https://kit.svelte.dev/docs/introduction) project which I have used to experiment with and
learn about various Svelte features and SSR.

The app also includes a SvelteKit + Firebase v10 implementation of the age-old [TodoMVC](http://todomvc.com) demonstration app where I have
added [Firebase Authentication](https://firebase.google.com/products/auth) and the [Firebase Realtime Database](https://firebase.google.com/products/realtime-database) for persistence of the todos.


## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Firebase setup

You will need to setup and configure your Firebase project to provide both Authentication and Realtime Database.  The configuration app settings are stored
in the `.env` file (as demonstrated in [dot_env](dot_env)) and are read in the `firebase.js` file.

The Firebase rtdb has an endpoint of `todos/` where the items are stored.


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
