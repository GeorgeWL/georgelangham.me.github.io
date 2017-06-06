# Based on the Creative portfolio theme for hugo

[![Buy Kishan B a coffee](https://img.shields.io/badge/%E2%98%95-Buy%20Kishan%20B%20a%20coffee-blue.svg)](https://www.paypal.me/kishansh/5)

Creative portfolio is a clean and elegant template mainly made for designers and creatives but can be easily transformed into a generic website.

# georgelangham.me.github.io

This site is a Static Generated Site, made with [Hugo](https://gohugo.io) and Automatically Deployed from a git repository using [Forestry.io](//Forestry.io)

The power of Hugo is that through the use of layout files, every div can easily be created or edited through HTML/CSS/JavaScript and then Injected into place by the program.

The simplest way to think of it is that every page is a template with empty spaces (assigned by the user or the theme) for Formatted Text to go into. And Hugo is the Glue which sticks that Text in place.

I’m currently using a heavily modified version of the the [Hugo Creative Portfolio Theme](https://github.com/kishaningithub/hugo-creative-portfolio-theme) by Github User [@Kishaningithub.](https://github.com/kishaningithub)

# The Current Deployment method is as such:

## For Content Changes

Login to the Forestry.io Headless CMS ([headlessCMS.org](//headlesscms.org) for a definition of what defines a Headless CMS)

Edit or Create Markdown Files using existing Templates, 

Forestry automatically pushes these to the Content folder, runs Hugo, which converts markdown in /Content/ to html and places them in the [/static](https://github.com/GeorgeWL/georgelangham.me.github.io/tree/dev/static) folder of the dev branch.

Forestry Publishes the contents of the /static/ folder in the dev branch of the Git onto the master branch as HTML/CSS/JavaScript files.

All contents of the master branch are automatically served as Webpages by Github Pages, due to a setting turned on in the options of the repository.

## Template and Layout Changes

deployed via opening the [/Layouts/](https://github.com/GeorgeWL/georgelangham.me.github.io/tree/dev/layouts) folder inside of the dev branch of the repository.

editing the [/partials/](https://github.com/GeorgeWL/georgelangham.me.github.io/tree/dev/layouts/partials), [/widgets](https://github.com/GeorgeWL/georgelangham.me.github.io/tree/dev/layouts/partials/widgets), /shortcodes or any of the other named templates.   Or potentially creating a new template file.

opening command prompt inside of the / folder

running the command hugo --theme [Theme-Name] once

syncing the changes back to the dev branch.

Forestry automatically publishes the new contents of the /static folder onto the Master branch

e.g.

about/single.html for editing the single page template of about.

e.g.

partials/sidebar.html for editing just the sidebar.

e.g.

portfolio/list for editing the grouped page template of Portfolio.


## License

This port is released under the MIT License. Check the [original theme license](https://bootstrapious.com/p/creative-portfolio) for additional licensing information.

## Thanks

Thanks to [Steve Francia](https://github.com/spf13) for creating Hugo and the awesome community around the project. And also thanks to [Bootstrapious](http://bootstrapious.com/) for creating this awesome theme and [Kishan B](https://github.com/kishaningithub) for Porting it to Hugo.
