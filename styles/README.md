# Conduit SASS

This repository contains the SASS files required for frontend apps that adhere to the Conduit ProductionReady spec. The entry file `scss/conduit.scss` not only includes all Conduit specific styles, but also includes a version of Bootstrap 4 Alpha. This ensures all future versions of Conduit SASS are guaranteed to work, as B4 is in alpha and subject to frequent changes.

## Using it in a project

Run `npm install conduit-sass --save`, then in your project's local SASS file `@import 'node_modules/conduit-sass/scss/conduit.scss';`

## Modifying SASS/HTML

We've included a simple gulp task that assists in viewing & modifying the templates & SASS. To preview and modify Conduit SASS & HTML with livereload, do the following:

1. Pull repo
2. npm install
3. Run `gulp`

Your browser should open automatically with livereload enabled. Whenever you edit SASS files in the `scss/` folder or modify HTML files in the `pages/` folder, gulp will regenerate & place a single CSS file and the individual HTML files into the `app/` folder.
