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

Run the `babel` script using npm.


~~~~~~shell
npm run babel
~~~~~~

Add the built `bundle.js` file to a project `.html` file.


~~~~~~shell
<script src="build/main.bundle.js"></script>
~~~~~~

Start `http-server`.

~~~~~~shell
npm start
~~~~~~

Now accessible is the `http-server` through port `8081`.

Point your browser to `http://localhost:8081` to find the project.

Or use curl to test the URL.

~~~~~~shell
curl http://localhost:8081
~~~~~~
