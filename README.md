# Demonstration of chrome livereloading bug.
POC for a bug in chromes sourcemaps when using livereload.
Some source forked from: https://github.com/Browsersync/recipes/tree/master/recipes/server

**Step 1**: Clone this entire repo
```bash
$ git clone https://github.com/TristanBrotherton/chrome_live_reload_bug.git
```

**Step 2**: Move into the directory containing this example
```bash
$ cd chrome_live_reload_bug
```

**Step 3**: Install dependencies
```bash
$ npm install
```

**Step 4**: Run the example
```bash
$ npm start
```

### Additional Info:



To see the live-updating and CSS injecting, simply perform changes to either `index.html` or `css/main.css`

### Preview of `app.js`:
```js
/**
 * Require Browsersync
 */
var browserSync = require('browser-sync');

/**
 * Run Browsersync with server config
 */
browserSync({
    server: "app",
    files: ["app/*.html", "app/css/*.css"]
});
```
