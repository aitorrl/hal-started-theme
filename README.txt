##### Hal - Starter theme based in bootstrap for Drupal 8

## Requirements
Node.js
Gulp.js

-Included Hal theme
Gulp
Bower
Libsass
Gulp autoprefixer
browser-sync

## Install & Run
-Install
Need Drupal bootstrap theme (https://www.drupal.org/project/bootstrap) installed in:
/sites/themes/contrib/

Place Hal starter theme in:
/sites/themes/custom/

-Into theme Hal directory:
npm install (install dependencies)
Edit gulpfile.js to config your local environment;
run 'gulp'


## Notes:

-Stylesheets remove, override Ej:
in hal.info.yml archive add:
-----------------
stylesheets-remove:
  - core/assets/vendor/normalize-css/normalize.css
  - core/modules/system/css/system.theme.css
------------------
More info for stylesheets remove, override etc. (D8 section):
https://www.drupal.org/node/1876600


-Debugging Twig templates
in sites/default/services.yml edit:
-----------------
parameters:
  twig.config:
    debug: true
-----------------
More info:
https://www.drupal.org/node/1906392
