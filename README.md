# vite_tailwinds_projects


How setup a project using Vite and Tailwind

1 - npm create vite@latest name_of_app

2- cd name_of_app

3- npm install

4-npm run dev   (see app)

5- npm install -D tailwindcss postcss autoprefixer

6- npx tailwindcss init -p --full

7- create src folder add  :  input.css   and add:          

@tailwind base;
@tailwind components;
@tailwind utilities;


8-  npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

9-  src/index.html

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

10- In tailwind.config.js  add :

content: [ "src/index.html" ] 

