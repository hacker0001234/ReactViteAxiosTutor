# ReactViteAxiosTutor

САМЕ ГЛАВНЕ НЕ ЗАБУДЬ РОЗРІШИТЬ ЛОСТУП ДЛЯ ЗАПРОСОВ З РЕАКТА НА БЕКЕНД(добав в бекенд cors.java)


пререходиш в папку де потрібно підключити 

cd name

npm create vite@latest . 

вибираєш реакт і якшо джава скріпто javascript 

npm install

npm install axios


запуск (тільки перервірь чи ти в тій папкі а то буде ошибка cd name)

npm run dev (якшо ти запустив проект і хочеш отмінить то заходиш в термінал і ctrl + c)



Дополнітельно:

для роботи з рутами(шоб було багато страніц)

npm install react-router-dom


npm install @stripe/stripe-js(бібіотека для страйп оплати)


кукі бібліотека npm install js-cookie
 

бібліотека для готових компонентів (https://v4.mui.com/ru/getting-started/usage):
npm install @mui/material @emotion/react @emotion/styled

npm install @mui/icons-material @mui/material @emotion/react @emotion/styled

npm install @fortawesome/react-fontawesome @fortawesome/free-regular-svg-icons @fortawesome/free-solid-svg-icons

npm install js-base64 для декодінгу або закодування 


 <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap" />
 <link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />


installing a heroUI:
first install vite 

second 
npm install -D tailwindcss@3 postcss autoprefixer
npx tailwindcss init -p

third instead of content: [] in tailwind.config,js place follow code :
content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],

  fourth in index.css remove all and place this:
  @tailwind base;
@tailwind components;
@tailwind utilities;

fiveth 
npm install @heroui/react framer-motion

sixth in tailwind.cofig.js in content place "./node_modules/@heroui/theme/dist/**/*.{js,ts,jsx,tsx}", DONT REMOVE CODE WHICH ALREADY WAS THERE
after in tailwind.config.js add on the top const {heroui} = require("@heroui/react");
and instead of plugins place 
  darkMode: "class",
  plugins: [heroui()],

tailwind.config.js will be like that:
const {heroui} = require("@heroui/react");

/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
    "./node_modules/@heroui/theme/dist/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  darkMode: "class",
  plugins: [heroui()],
}

after go to main.jsx and import {HeroUIProvider} from "@heroui/react";
and wrap ur project in HeroUIProvider like:
  <HeroUIProvider>
      <YourApplication />
    </HeroUIProvider>

    and it will look like:
    

import { createRoot } from 'react-dom/client'
import './index.css'
import App from './App.jsx'
import {HeroUIProvider} from "@heroui/react";

createRoot(document.getElementById('root')).render(
  <HeroUIProvider>
    <App />
  </HeroUIProvider>,
)


npm install event-source-polyfill - это типо EventSource но из куками тоесть куки передаються 
