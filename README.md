1. Create package.json file with default options ->
    npm init –y
2. Install Tailwind CSS ->
    npm install tailwindcss
3. Install AutoPrefixer -> 
    npm install autoprefixer
4. Create public Folder then inside public folder create index.html. public/index.html where you can write your html code.
5. Create src Folder then inside src folder create tailwind.css file (You can change file name). src/tailwind.css file is used to write tailwind directives and custom CSS.
6. Open src/tailwind.css file then write code -> 
        @tailwind base;
        @tailwind components;
        /* Write Custom CSS */
        @tailwind utilities;
7. Create Build Script which will compile src/tailwind.css file to actual css file. To do this, Open package.json file then write code -> 
        "scripts": {"build": "tailwindcss build ./src/tailwind.css -o ./public/tailwind.css"}
8. Run the script -> 
        npm run build
  This will generate a compiled tailwind.css file inside public folder. This public/tailwind.css file has actual tailwind css code. You should not modify this file.
9. Done -> 
   Note - If we are working on a small project which doesn’t use any kind of framework then we should use “Tailwind CSS without PostCSS” process to install tailwind.
