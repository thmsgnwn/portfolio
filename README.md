Build Portofolio using Tailwind Css 3

## Instalation

```
https://tailwindcss.com/docs/installation

```

### Terminal

```
npm install -D tailwindcss
npx tailwindcss init
```

### Change script from tailwind.config.js

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["index.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### Make folder src/input.css

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Make folder dist/output.css and dist/img/{input file image}

```
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

### Develop & Build App

to dev `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`
and
to build `npx tailwindcss  -o ./public/css/final.css --minify`
