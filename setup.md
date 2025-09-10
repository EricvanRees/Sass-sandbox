**Environment Setup with Node Sass**

This setup is required to compile scss files

1) Make sure NodeJS is installed locally by checking its version with "npm --version" in the terminal.
2) Create a package.json file for your project with "npm init -y"
3) Install Sass so it is listed as a project dependency in the package.json file, run "npm install node-sass". A folder named "node_modules" is created.
4) Create a script to simply run "npm run sass" in the terminal. Add the following to the package.json file:   
"scripts": {
    "sass": "node-sass -w scss/ -o dist/css/ --recursive"
  }
5) Create a "scss" folder to store all scss files. Create a "dist" folder for all project files. 
6) Run "npm run sass" to constantly watch the "scss" folder and the files within it. These will be compiled into the "dist" folder.
7) Create a main.scss file in the "scss" folder. This is where you write Sass, which gets compiled into the main.css file automatically.
8) Create an index.html file in the "dist" folder, link to the "css/main.css" file in the HTML file.


