# Testing Your Style Guide and Theme in Drupal 8 - Demo Repository

This serves as a playground to experiment with the concepts covered in the 'Testing Your Style Guide and Theme in Drupal 8' talk.  The related slides can be viewed at [http://brianperryinteractive.com/testing-d8-theme](http://brianperryinteractive.com/testing-d8-theme) or in the gh-pages branch of this repository.  At the moment, this only includes a single simple example, but I'm hoping to expand this over time.

### Installing Drupal

Checkout this repository and follow the standard Drupal 8 installation process.  If installing from the Web interface you may need to manually request install.php [due to this issue](https://www.drupal.org/node/728702).

### Enabling Testing Walkthrough Theme

- First, enable the components module (this is required by the testing_walkthrough theme)
- Then enable the Testing Walkthrough theme.

### Todo

- Export config to:
  - Enable components module (or make it a dependency of the testing_walkthrough theme)
  - Enable testing_walkthrough theme
  - Set theme config
    - Disabled logo image
    - Disabled blocks - footer menu, main navigation, user account menu
