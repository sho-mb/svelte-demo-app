# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/main/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
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

## Memo

Syntax 
```
For loop : {#each list as item} {/each}

if : {#if condition} {else if condition} {else} {/if}
```

Css with logic
```
class = {"some css " + (condition ? " colot:red" : " ")}
```
* Add space before css in condition

Inport item prop form parents

```
<script>
export let valiable; <- This is defineProps in vue

</script>

```

Structure 
* All component goes to components folder (need to be created)
* routes : Page and layout (Page contain top view, Add more route create dir. name will be path)
  * Ex: About dir (contain page.svelte) => localhost/about
* In page shoule be only components
* +layout: Add <slot> tag and you can wrapp with specific css and add header footer etc
* App.css contain common css such as font family, reset css, etc... also tailwind as well.
* Tailwind has specific way to install fot svelte go to check as below
  * https://tailwindcss.com/docs/guides/sveltekit



