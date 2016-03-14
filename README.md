# [Sass Bootstrap v3.3.6](http://getbootstrap.com)

Bootstrap is a sleek, intuitive, and powerful front-end framework for faster and easier web development, created and maintained by [Mark Otto](http://twitter.com/mdo) and [Jacob Thornton](http://twitter.com/fat).

This is the Sass version of Bootstrap. A port of Bootstrap from Less to Sass. This project is focused on being a 1:1 port of the original. Please do not submit issues or pull requests for issues with Bootstrap itself. Those should be pushed upstream in the Less version.

To get started, check out [http://getbootstrap.com](http://getbootstrap.com)!



##Usage

This is a module for better use of bootstrap in silverstripe projects.

To download use:
 composer require purezero/module_bootstrap

This will download the package into the themes directory of your silverstripe project.
###Just CSS and javascript

If you just need to link the code to use the css selectors, this can be done by linking the files found in the dist folder on page.php, this can be done through
        Requirements::javascript('themes/module_bootstrap/dist/js/bootstrap.min.js');
        Requirements::css('themes/module_bootstrap/dist//css/bootstrap.min.css');

###Using SASS for variables and mixins

I am not sure on what best practise is here, but I create a new bootstrap.scss in my themes directory and import module_bootstrap/lib/_boostrap.scss into that file.
So when I compile my other code it will compile bootstrap as well.

With regards to mixins and other files that would be nice in my SASS I would just import the needed files into the scss file that needs it.

## Copyright and license

Copyright 2012 Twitter, Inc under [the Apache 2.0 license](LICENSE).
