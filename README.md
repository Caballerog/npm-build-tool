# npm-tool
Using npm as a build tool instead of Grunt or Gulp.

# Features

- Automatically lint your scripts.
- Automatically minify your HTML, CSS and JS using htmlminifier, css-clean and uglifyJS2.
- CSS Autoprefixing using PostCSS.
- Awesome image optimization using imagemin (You can use subfolder)
- Automatically wire-up dependencies installed with Bower using wiredep.
- Automatically create your JavaScript documentation using jsDoc.
- Automatically create a hashmark in your new JavaScript file and CSS file for avoid cache problems.

# Getting started
- Install dependencies: `npm install`.
- Configure your variables in `package.json`.
- Run `npm run build` to build your production build.

# Configuration in package.json
- `"main"`: Index file of your app (Default src/).
- `"config"`: JSON Object with configuration's object.
 - `"src"`: Top level folder of your source code.
 -  `"srcJS"`: Folder of your JavaScript source code (Default src/****/*.js).
 -  `"srcCSS"`: Folder of your CSS source code. (Default src/****/*.css).
 -  `"srcImages"`: Folder of your images (Default src/assets/images/).
 -  `"distJS`: Production folder of your JavaScript (Default dist/js/).
 -  `"distCSS`: Production folder of your CSS (Default /dist/css/).
 -  `"distImages`: Productio folder of your images (Default dist/images/).
 -  `"distDoc`: Production folder of your JavaScript documentation (Default dist/doc/).

# Usage

-  `npm run build`: Build your production app.
-  `npm run build:watch`: Build your production app and watcher any change in your code.
-  `npm run build:images`: Minify your images.
-  `npm run clean`: Clean your production app.
-  `npm run clean:css`: Clean your CSS folder in your production app.
-  `npm run clean:js`: Clean your JS folder in your production app.
-  `npm run clean:images`: Clean your images folder in your production app.
-  `npm run lint:js`: Run Lint in your source JS code.

# TO-DO
- Integrated liveReload.
- JavaScript dependencies Script (e.g. using uglifyJS2).
- Preprocessador CSS (e.g. using Less/SASS)
- AngularJS dependencies inyection.

