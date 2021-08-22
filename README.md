# lock
This is a script which uses a background image, resizes it to show correctly on any multimonitor setup.

The idea for this project was shamelessly copied from [guimeira](https://github.com/guimeira)'s [i3lock-fancy-multimonitor](https://github.com/guimeira/i3lock-fancy-multimonitor).

It uses [ImageMagick](http://www.imagemagick.org/) to resize the [background image](./img/background.png). You can replace this image to change background.

By using information from [xrandr](http://www.x.org/wiki/Projects/XRandR/) and basic math, this script supports multiple monitor setups, displaying the background image on all screens.

It caches the generated image for different screen sizes and xrandr output. So even though first `lock` command will take a second to finish, subsequent `lock` will be lighting fast.

![Screenshot](./example.png)
