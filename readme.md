# Testing Your Style Guide and Theme in Drupal 8 - Demo Repository

This serves as a playground to experiment with the concepts covered in the 'Chasing the Dream of Style Guide Development in Drupal 8' or 'Testing Your Style Guide and Theme in Drupal 8' talks.  The related slides can be viewed at [http://brianperryinteractive.com/testing-d8-theme](http://brianperryinteractive.com/testing-d8-theme) or in the docs directory of this repository.  At the moment, this only includes a single simple example, but I'm hoping to expand this over time.

### Installing Drupal

Checkout this repository and follow the standard Drupal 8 installation process.  If installing from the Web interface you may need to manually request install.php [due to this issue](https://www.drupal.org/node/728702).

### Import Site Configuration

- To enable the testing theme and related site configuration, import the configuration located at _config/sync
https://www.drupal.org/docs/8/configuration-management/managing-your-sites-configuration

### Content

- In the future, example content will be included with this repository.  But for now, creating 3 article nodes with a Title, Image and Body will cover the example.

### Generating KSS Style Guide

__Prerequisites:__

- Install node.js globally.
     - On OS X I'd suggest using homebrew to install node - http://blog.teamtreehouse.com/install-node-js-npm-mac
     - Or https://docs.npmjs.com/getting-started/installing-node
 - From themes/neato_refills run:

 npm install

__Generating the style guide:__

With the steps above completed gulp will watch for changes in your sass or twig templates and rebuild the style guide when any changes are made.

To start gulp, run the following from themes/neato_refills:

grunt

The style guide will be built in themes/neato_refills/styleguide

### Visual Regression Tests

- install GraphicsMagick as outlined in the readme here: https://github.com/webdriverio/webdrivercss
- run npm install as listed above
- ./node-modules/.bin/selenium-standalone install
- ./node_modules/.bin/selenium-standalone start (starts selenium)
- in tests/wdio-tests.js update the .url() value
- execute tests with node tests/wdio-tests.js

