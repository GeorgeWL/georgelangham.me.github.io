+++
date = "2015-11-07T10:37:00Z"
image = "/uploads/2017/05/26/screenshot-homepages.shu.ac.uk-2017-05-26-13-00-07_iphone_white_side2.png"
showonlyimage = true
title = "JQuery-UI Project"
weight = 9

+++
As part of my University Course, after reading and researching the documentation of the JQuery-UI Mobile framework, a short project was set to create a single file site which uses JQuery-UI Mobile elements.

All of the pages of this site are run from the same file (index.html) with CSS, Images and JavaScript files called in when necessary. Rather than each page being a file, it is a `<div>` with the `data-role` of `page`
<!--more-->

In the example of code, note how pages are defined in `data-role` elements.

```
<div id="deluxe" data-role="page">
	<div class="ui-corner-top ui-overlay-shadow ui-header ui-bar-a" role="banner">
		 <a href="#rooms" data-icon="delete" data-iconpos="notext" class="ui-btn-right ui-btn ui-btnicon-notext
		ui-btn-corner-all ui-shadow ui-btn-up-a" title="Close" data-theme="a"datatransition="pop" data-direction="reverse">
			 <span class="ui-btn-inner ui-btn-corner-all">
			 <span class="ui-btn-text">Close<span>
			 <span class="ui-icon ui-icon-delete ui-icon-shadow"><span>
		 </span>
		 </a>
		<h1 class="ui-title" tabindex="0" role="heading" aria-level="1">The deluxe Room</h1>
	</div>
	<div data-role="content">
		<h1>The deluxe Room </h1>
		<img src="images/.deluxe.jpg" alt="Deluxe Room" />
		...
</div>

```