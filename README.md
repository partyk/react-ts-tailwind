# react-ts-tailwind

Instalační postup

1) Instalace vite
```
npm init vite@latest
```
2) Otevření a spušttění projektu.
```
cd react-ts-tailwind
npm install
npm run dev 
```
3) Isntalace tailwindcss postcss autoprefixer
```
npm i -D tailwindcss postcss autoprefixer
```
4) Integrace tailwindcss. Vytvoření konfigurace
```
npx tailwindcss init -p
```
- Vytvoří konfiguráky pro tailwind
```
postcss.config.js
```
```
tailwind.config.js
```
5) Doplni do **tailwind.config.js** lokaci kde se bude s tailwindem pracovat
```
/** @type {import('tailwindcss').Config} */
export default {
    content: [
        './index.html',
        './src/**/*.{js,ts,jsx,tsx}',
    ],
    theme: {
        extend: {},
    },
    plugins: [],
};
```
6) **index.css**  přejmenuji na **index.scss** a nainstaluji sass doplni linky na tailwind
```
npm i -D sass
```
index.scss
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
7) Spustím vite s portem 4000
```
npx vite --port 4000

nebo

npm run dev
```
