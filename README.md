[![Build Status](https://travis-ci.org/tcatm/meshviewer.svg?branch=master)](https://travis-ci.org/tcatm/meshviewer)

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

# Preparing for installation

There are some hooks and common problems when you install for example on debian:

install nodeJS that includes npm with your package manager, for example `apt-get`

    sudo apt-get install nodejs

On debian there is no need of the often installed packet `node` and grunt will not work with it installed:

    sudo apt-get remove --purge node
    sudo ln -s /usr/bin/nodejs /usr/bin/node

# Installing dependencies

    npm install bower
    npm install grunt-cli
    npm install sass
    npm install
    bower install

# Building

You may want to tweak `lib/config.js` to point to your data files. If it's
served from a different domain, remember to [enable CORS] on your
webserver. Enabling GZip will reduce bandwidth consumption.

Just run:

    grunt

This will generate `build/` containing all required files.

[enable CORS]: http://enable-cors.org/server.html
