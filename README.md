# NuxtJS3 + TailwindCSS Setup

This repo just shows how to get a simple landing page up and running with NuxtJS V3 and TailwindCSS.

- [NuxtJS](https://nuxtjs.org/)
- [TailwindCSS](https://tailwindcss.com/)
- [Pexels](https://www.pexels.com/)

# Demo

https://advanced-homes.behonbaker.com/

## Steps

[x] : Create Nuxt App with command

```bash
npx nuxi init nuxt3-app
```

[x] : Install TailwindCSS

```bash
npm install -D tailwindcss postcss autoprefixer && npx tailwindcss init
```

[x] : Add postcss config to your `nuxt.config.ts`

```js
export default defineNuxtConfig({
	// ...
	postcss: {
		plugins: {
			tailwindcss: {},
			autoprefixer: {},
		},
	},
	//...
});
```

[x] : Add Content paths to you `tailwind.config.js`

```js
module.exports = {
	// ...
	content: [
		"./components/**/*.{js,vue,ts}",
		"./layouts/**/*.vue",
		"./pages/**/*.vue",
		"./plugins/**/*.{js,ts}",
		"./nuxt.config.{js,ts}",
	],
	// ...
};
```

[x] : Create main CSS file and add it to your `nuxt.config.ts`

```bash
mkdir -p assets/css && touch assets/css/main.css
```

```js
export default defineNuxtConfig({
	// ...
	css: ["~/assets/css/main.css"],
	//...
});
```

[x] : Add tailwind to CSS file

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

[x] : Install Tailwind CSS VS Code extension

https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss

## Next Steps

Create your landing page and start building your app.
