Starting an ECMAScript Project
==============================

~~~~~~shell
# Create the project directory.
mkdir some_project
cd some_project

# Initialize the project.
npm init

# Install npm packages for babel (ES6 support).
npm install babel-cli babel-core --save-dev
npm install babel-preset-es2015 --save-dev

# Install a local web server.
npm install http-server --save-dev
~~~~~~

Modify `package.json` as follows:

~~~~~~shell
"scripts": {
    "babel": "babel --presets es2015 js/main.js -o build/main.bundle.js",
    "start": "http-server"
},
~~~~~~
