+++
date = "2017-05-26T12:26:33+00:00"
image = "/uploads/2017/05/26/Gwl.png"
showonlyimage = false
title = "Georgelangham.me"
weight = 1

+++
This site is a Static Generated Site, made with [Hugo](https://gohugo.io) and Automatically Deployed from a [git repository](https://github.com/GeorgeWL/georgelangham.me.github.io) using [Forestry.io](https://Forestry.io)

The power of Hugo is that through the use of layout files, every  div can easily be created or edited through HTML/CSS/JavaScript and then Injected into place by the program.
<!--more-->

The simplest way to think of it is that every page is a template with a single empty space in the middle for Formatted Text to go into. And Hugo is the Glue which sticks that Text in place.

I'm currently using a heavily modified version of the the [Hugo Creative Portfolio Theme](https://github.com/kishaningithub/hugo-creative-portfolio-theme) by Github User Kishaningithub.

The Current Deployment method is as such:

## For Content Changes

1. Login to the Forestry.io Headless CMS ([headlessCMS.org](headlesscms.org) for a definition of what defines a Headless CMS)

1. Edit or Create Markdown Files using existing Templates

1. Forestry builds these pages into HTML and places them in the `/public` folder of the `dev` branch

1. Forestry Publishes the contents of the `/public` folder in the `dev` branch of the Git onto the `master` branch

1. All contents of the `master` branch are automatically served as Webpages by Github Pages, due to a setting turned on in the options of the repository.

## Major Template and Layout Changes

deployed via opening the `/Layouts` folder inside of the dev branch of the repository, using Github Desktop and then:

1. editing the `/partials`, `/widgets`, `/shortcodes` or any of the named templates

1. opening command prompt inside of the `/` folder

1. running the command `hugo --theme [Theme-Name]` once

1. syncing the changes back to the dev branch.

1. publishing the contents of the `/public` folder onto the Master branch

* e.g. `about/single.html` for editing the single page template of about.

* e.g. `partials/sidebar.html` for editing just the sidebar.

* e.g. `portfolio/list` for editing the grouped page template of Portfolio.