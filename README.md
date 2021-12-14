# vue3-dashboard

----------------------

Resources:

* [Tailwind](https://tailwindcss.com/docs/installation)
* [Dialog (Modal)](https://headlessui.dev/vue/dialog)
* [Hero Icons](https://heroicons.com) + [GitHub](https://github.com/tailwindlabs/heroicons)
* [Layout](https://tailwindui.com/components/application-ui/application-shells/stacked)

---------------------

```
yarn add @headlessui/vue
yarn add @heroicons/vue
yarn add tailwindcss postcss autoprefixer

```

``` 
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init

```

tailwind.config.js

```js
module.exports = {
    content: ["./src/**/*.{html,js}"],
    theme: {
        extend: {},
    },
    plugins: [],
}
```

postcss.config.js

```js
module.exports = {
    plugins: {
        tailwindcss: {},
        autoprefixer: {},
    }
}
```

main.css tailwind.css.css

```css 
@tailwind base;
@tailwind components;
@tailwind utilities;
```

index.html

``` html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/main.css" rel="stylesheet">
</head>
```

[main.js](src/main.js)

```js 
import './assets/css/tailwind.css';
import './assets/css/main.css';

```

You can import the css file on [App.vue](/src/App.vue), inside the style tag.

```html

<style>
    @import './assets/css/tailwind.css';
    @import './assets/css/main.css';
</style>
```

---------------------

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Lints and fixes files

```
npm run lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
