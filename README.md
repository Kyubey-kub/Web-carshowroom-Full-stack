Car Showroom Project
This repository contains the Frontend and Backend for the Car Showroom project, built with modern web technologies.
Frontend
Overview
The Frontend is built using React + TypeScript + Vite, providing a minimal setup with Hot Module Replacement (HMR) and ESLint rules.
Installed Packages
The following packages are installed in the Frontend project (car-showroom-frontend@0.0.0):

@eslint/js@9.22.0
@react-three/drei@10.0.4
@react-three/fiber@9.1.0
@types/react-dom@19.0.4
@types/react@19.0.10
@vitejs/plugin-react@4.3.4
autoprefixer@10.4.21
axios@1.8.4
chart.js@4.4.8
eslint-plugin-react-hooks@5.2.0
eslint-plugin-react-refresh@0.4.19
eslint@9.22.0
framer-motion@12.6.2
globals@15.15.0
postcss@8.5.3
react-chartjs-2@5.3.0
react-dom@19.0.0
react-router-dom@7.4.1
react@19.0.0
tailwindcss@3.4.17
three@0.174.0
typescript-eslint@8.26.0
typescript@5.7.3
validator@13.15.0
vite@6.2.1

Setup Details
This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.
Currently, two official plugins are available:

@vitejs/plugin-react uses Babel for Fast Refresh
@vitejs/plugin-react-swc uses SWC for Fast Refresh

Expanding the ESLint Configuration
If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:
export default tseslint.config({
  extends: [
    // Remove ...tseslint.configs.recommended and replace with this
    ...tseslint.configs.recommendedTypeChecked,
    // Alternatively, use this for stricter rules
    ...tseslint.configs.strictTypeChecked,
    // Optionally, add this for stylistic rules
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})

You can also install eslint-plugin-react-x and eslint-plugin-react-dom for React-specific lint rules:
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})

Backend
Overview
The Backend is built using Node.js with TypeScript and Express, providing API endpoints and database integration for the Car Showroom project.
Installed Packages
The following packages are installed in the Backend project (car-showroom-backend@1.0.0):

@types/bcryptjs@3.0.0
@types/cors@2.8.17
@types/date-fns@2.6.3
@types/express@5.0.1
@types/jsonwebtoken@9.0.9
@types/multer@1.4.12
@types/node@22.13.14
@types/nodemailer@6.4.17
@types/validator@13.12.3
@types/ws@8.18.1
bcryptjs@3.0.2
cors@2.8.5
date-fns@4.1.0
dotenv@16.4.7
express@4.21.2
jsonwebtoken@9.0.2
multer@1.4.5-lts.2
mysql2@3.14.0
nodemailer@6.10.1
nodemon@3.1.9
ts-node@10.9.2
typescript@5.8.2
validator@13.15.0
ws@8.18.1

Setup Details
The Backend leverages Express for routing, MySQL2 for database interactions, and TypeScript for type safety. Environment variables are managed with dotenv, and nodemon is used for development hot-reloading.
Getting Started

Clone the Repository:
git clone https://github.com/Kyubey-kub/web-carshowroom-Frontend.git
git clone https://github.com/Kyubey-kub/web-carshowroom-Backend.git


Install Dependencies:

For Frontend:cd web-carshowroom-Frontend
npm install


For Backend:cd web-carshowroom-Backend
npm install




Run the Project:

For Frontend:npm run dev


For Backend:npm run dev





Contributing
Feel free to submit issues or pull requests to improve the project.
License
This project is licensed under the MIT License - see the LICENSE file for details.
