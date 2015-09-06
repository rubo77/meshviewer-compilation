[![Build Status](https://travis-ci.org/tcatm/meshviewer.svg?branch=master)](https://travis-ci.org/tcatm/meshviewer)

# This is just a fork

If you want to fork this project, please use the main fork:
https://github.com/ffnord/meshviewer/

---

# Meshviewer

Meshviewer is a frontend for
[ffmap-backend](https://github.com/ffnord/ffmap-backend).

# Screenshots

![](doc/mapview.png?raw=true)
![](doc/graphview.png?raw=true)
![](doc/allnodes.png?raw=true)
![](doc/links.png?raw=true)
![](doc/statistics.png?raw=true)

# Dependencies

- npm
- bower
- grunt-cli
- Ruby and Sass

# Installing dependencies

    npm install
    bower install

# Building

You may want to tweak `lib/config.js` to point to your data fils. If it's
served from a different domain, remember to [enable CORS] on your
webserver. Enabling GZip will reduce bandwidth consumption.

Just run:

    grunt

This will generate `build/` containing all required files.

[enable CORS]: http://enable-cors.org/server.html
