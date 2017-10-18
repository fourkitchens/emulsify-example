## Emulsify Example
This is a basic views gallery example.

## Prerequisites
- Drush 9.x is installed on your local machine

## Setup
1) Create a new Acquia Dev Desktop Drupal 8.4.0 site
2) Delete the code that it creates and use this repository
3) Copy your ~/.acquia/DevDesktop/DrupalSettings file to sites/default/settings.local.php
4) Consider adding additional options to settings.local.php see example.settings.local.php file for examples
5) Copy your Acquia drush aliases ~/.acquia/DevDesktop/Drush/Aliases/aliases.drushrc.php to your ~/.drush/devdesktop.aliases.drushrc.php
6) You can now see your devdesktop sites by using `drush9 sa @devdesktop`
7) Edit your `$settings['trusted_host_patterns']` if you aren't using `emulsify-example.dd` as your domain.
8) DON'T do this with produciton data but since this is an example you can import the database now
9) Change directories to the root of this project and type `gzip -dc emulsify_example.sql.gz | drush9 @devdesktop.loc.emulsify-example sqlc`
10) Visit `emulsify-example.dd:8083`
11) To login go to `emulsify-example.dd:8083/user`
12) Type the very secure login information.  User: admin Pass: admin

## Demo
- http://emulsify-example.dd:8083/gallery
- `cd ~/devdesktop/emulsify-example/themes/custom/demo`
- `yarn start`
- `http://localhost:3000/pattern-lab/public/`
- `atom ~/devdesktop/emulsify-example`
