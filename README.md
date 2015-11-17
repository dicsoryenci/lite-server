# lite-server

Lightweight *development only* node server that serves a web app, opens it in the browser, refreshes when html or javascript change, injects CSS changes using sockets, and has a fallback page when a route is not found.

## Get Started

### Serve the current folder and `./index.html`
Serve from the current folder and open (browse to) the default file (usually index.html) in that folder.

`lite-server`

### Serve the current folder and `./src/index.html`
Serve from the current folder and open (browse to) the default file (usually index.html) in the `src` folder.

`lite-server --open src`

### Serve and log all options

`lite-server --verbose`


### port
Sets the port to serve. Defaults to 3000.

`--port 3000`

### open
Which folder to holds the `index.html`. Defaults to `./`

`--open src`

### files

Array of file patterns to watch. Defaults to all html, css and js.

`--files '/**/*.html' '/**/*.css' '/**/*.js'`

### baseDir

Folder (or collection of folders) to serve. Defaults to `./`. Use this when you want to specify which folders you want to serve assets from.

`--baseDir './'`

### fallback

File to serve when a route is not found. Useful for SPAs. Defaults to `source` folder + `/index.html`.

`--fallback '/src/index.html'`
