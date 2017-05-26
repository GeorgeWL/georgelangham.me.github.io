+++
date = "2015-11-07T10:37:00+00:00"
image = "/uploads/2017/05/26/screenshot-homepages.shu.ac.uk-2017-05-26-13-00-07_iphone_white_side2.png"
showonlyimage = true
title = "JQuery-UI Project"
type = ""
weight = 9

+++


As part of my University Course, after reading and researching the documentation of the JQuery-UI Mobile framework, a short project was set to create a single file site which uses JQuery-UI Mobile elements.

All of the pages of this site are run from the same file (index.html) with CSS, Images and JavaScript files called in when necessary. Rather than each page being a file, it is a `&lt;div&gt;` with the `data-role` of `page`
<!--more-->

In the example of code, note how pages are defined in `data-role` elements.

```
&amp;lt;div id="deluxe" data-role="page"&amp;gt;
	&amp;lt;div class="ui-corner-top ui-overlay-shadow ui-header ui-bar-a" role="banner"&amp;gt;
		 &amp;lt;a href="#rooms" data-icon="delete" data-iconpos="notext" class="ui-btn-right ui-btn ui-btnicon-notext
		ui-btn-corner-all ui-shadow ui-btn-up-a" title="Close" data-theme="a"datatransition="pop" data-direction="reverse"&amp;gt;
			 &amp;lt;span class="ui-btn-inner ui-btn-corner-all"&amp;gt;
			 &amp;lt;span class="ui-btn-text"&amp;gt;Close&amp;lt;/span&amp;gt;
			 &amp;lt;span class="ui-icon ui-icon-delete ui-icon-shadow"&amp;gt;&amp;lt;/span&amp;gt;
		 &amp;lt;/span&amp;gt;
		 &amp;lt;/a&amp;gt;
		 &amp;lt;h1 class="ui-title" tabindex="0" role="heading" aria-level="1"&amp;gt;The deluxe Room&amp;lt;/h1&amp;gt;
	&amp;lt;/div&amp;gt;
	&amp;lt;div data-role="content"&amp;gt;
		&amp;lt;h1&amp;gt; The deluxe Room &amp;lt;/h1&amp;gt;
		&amp;lt;img src="images/.deluxe.jpg" alt="Deluxe Room" /&amp;gt;
		&amp;lt;p&amp;gt; Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod. Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
		cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
		&amp;lt;/p&amp;gt;
	&amp;lt;/div&amp;gt;
&amp;lt;/div&amp;gt;

```