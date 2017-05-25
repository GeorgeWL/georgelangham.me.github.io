+++
date = "2017-05-25T18:15:11Z"
image = "/uploads/2017/05/25/Gwl1.jpg"
showonlyimage = true
title = "Georgelangham.me"
type = ""
weight = 4

+++
This site a Static Generated Site, made with [Hugo](https://gohugo.io) and Automatically Deployed using [Forestry.io](https://Forestry.io)

Hugo makes use of partial html files and layout files, that inject the text content from markdown files into defined spaces and then builds as a project.

The simplest way to think of it is that every page is a template with a single empty space in the middle for Formatted Text to go into. 

And Hugo is the Glue which sticks that Text in place.

The Current Deployment method is as such.

## For Content Changes

1. Login to the Forestry.io Headless CMS (headlesscms.org for defintion of what defines a headless CMS)
1. Edit Markdown Files to Create New Text Posts using existing Templates
1. Forestry builds these pages into HTML
1. Forestry Publishes the contents of the `/public` folder in the `dev` branch of the Git onto the `master` branch
1. All contents of the `master` branch are automatically served as Webpages by Github Pages, due to a setting turned on in the options.

## Major Template Changes

deployed via opening the `/Layouts` folder inside of the dev branch of the Git, using Github Desktop and then:

1. editing the `/partials`, `/widgets`, `/shortcodes` or any of the named templates 
1. opening command prompt inside of the `/` folder
1. running the command `hugo --theme [Theme-Name]` once
1. syncing the changes back to the dev branch.
1. publishing the contents of the `/public` folder onto the Master branch

* e.g. `about/single.html` for editing the single page template of about. 
* e.g. `partials/sidebar.html` for editing just the sidebar.
* e.g. `portfolio/list` for editing the grouped page template of Portfolio.