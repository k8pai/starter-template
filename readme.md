
## Get Started 🚀

Clone the project

```bash
  git clone https://github.com/k8pai/tailwind-css.git
```

Go to the project directory

```bash
  cd tailwind-css
```

Install dependencies

```bash
  npm install
```

Generate compiled tailwind css

```bash
  npx tailwindcss -i ./src/css/index.css -0 ./dist/index.css
```

 ###### -i contains custom css path.
 ###### -o destination of the compiled css.

## To be noted 🗒️

#### Renaming files. 🔗

tailwind.config.js file, contains the paths to the source files.
Whenever a file is renamed or moved to another directory, paths should be updated as well.

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/{index.html, index.js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

#### Links 🔗

Compiled css files are to be linked instead of custom css files.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <link href="/dist/index.css" rel="stylesheet">
</head>
<body>
    <h1 class="text-3xl font-bold underline">
        Hello world!
    </h1>
</body>
</html>
```

### Get going now 🧑🏻‍💻
