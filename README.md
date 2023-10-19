
## Install Flowbite Tailwind CSS with Vite React, Vue, Svelte
[Flowbite](https://flowbite.com/docs/getting-started/react/)


Create your project
```bash
  npm create vite@latest
  cd my-project
```

Install Tailwind CSS    
```bash
  npm install -D tailwindcss postcss autoprefixer
  npx tailwindcss init -p
```

tailwind.config.js
```bash
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

index.css
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Install Flowbite
```bash
npm install flowbite flowbite-react
```

tailwind.config.js
```bash
module.exports = {

    plugins: [
        require('flowbite/plugin')
    ]

}
```

tailwind.config.js
```bash
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    './src/**/*.{js,jsx,ts,tsx}',
    'node_modules/flowbite-react/**/*.{js,jsx,ts,tsx}'
  ],
  theme: {
    extend: {},
  },
  // eslint-disable-next-line no-undef
  plugins: [require('flowbite/plugin')],
}
```


Run Project
```bash
npm run dev
```
