Overview
========
This directory stores a default theme for an Open edX instance.

We've organized the tree to mimic the directory structure of the edX
codebase so that it's easy to tell where the files will end up upon
deploy. We'll use a special settings file to set the template and
staticfiles paths properly to point to these files.

![Alt text](/default_theme_screenshot.jpg?raw=true "Open edX Default Theme Screenshot")

Theme Authoring
===============
To customize your theme:
- Fork this repository.
- Clone it into the 'themes' directory next to your edx-platform directory and
  rename the cloned directory to your new theme's name.
- Upload your own image assets.
- Edit the .scss file in static/sass/ and rename the file with your theme's name.
  It should be called `_<theme-name>.scss` now.
- Also edit the references to the image paths in the .scss file under the heading
  'CSS BG Images'.
- Edit the lms.envs.json file in edx-platform and set 'USE_CUSTOM_THEME' to true, and 'THEME_NAME' to your theme's name.


License
=======

The code in this repo is licensed under the Apache 2.0 License.
See [LICENSE.txt](LICENSE.txt) for more info.
