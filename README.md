#Get Started

1. Install Node 6. Need to run multiple versions of Node? Use nvm or nvm-windows
2. Clone this repository.
3. Make sure you're in the directory you just created. - cd react-redux
4. Install Node Packages. - npm install
5. Run the app. - npm start -s
6. This will run the automated build process, start up a webserver, and open the application in your default browser.
..* When doing development with this kit, this command will continue watching files all your files.
..* Every time you hit save the code is rebuilt, linting runs, and tests run automatically.
..* Note: The -s flag is optional. It enables silent mode which suppresses unnecessary messages during the build.

7. Disable safe write to assure hot reloading works properly.
8. Install React developer tools and Redux Dev Tools in Chrome.

#Having Issues? Try these things first:

..* Run npm install - If you forget to do this, you'll see this: babel-node: command not found.
..* Make sure the path doesn't include any spaces, or install the latest version of eslint-watch which adds support for paths containing spaces: npm install eslint-watch@2.1.13
..* Make sure you're running the latest version of Node. Or, use Node 5.12.0 if you're having issues on Windows. Node 6 has issues on some Windows machines.
..* Make sure files with names that begin with a dot (.babelrc, .editorconfig, .eslintrc) are copied to the project directory root. This is easy to overlook if you copy this repository manually.
..* Don't run the project from a symbolic link. It will cause issues with file watches.
..* Use path.resolve on all path references in both the dev and prod webpack.config. See this commit for an example.
..* Delete any .eslintrc in your user directory and disable any ESLint plugin / custom rules within your editor since these will conflict with the ESLint rules defined in the course.
..* Nothing above work? Delete your node_modules folder and re-run npm install.
