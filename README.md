Baffin CSS
==========

Baffin is a starting place CSS. No delusions of grandeur here&mdash;just a couple of SASS mixins that provide minimal typography and grid support to your stylesheets.

And the name? It's just someplace up north I heard of once.

Overview
--------

To include Baffin's default styling, include the following at the top of your project&rsquo;s SCSS source files: 

	@include baffin-typography();
	@include baffin-grid(12,2%);

Compile using SASS or use a parser to include the styles directly. You now have access to a number of helper classes, including:

### typography
* `.amp` &mdash; switch to prettier fonts for ampersands 
* `.assistive-text` &mdash; hide text *except* from screen readers and assistive devices
* `.caps` &mdash; switch type to all caps
* `.hidden-text` &mdash; hide text
* `.mobile-text` &mdash; hide text on non-mobile screens
* `.print-text` &mdash; hide text from printers (*note: text must be `display`ed manually*)
* `.smaller` &mdash; reduce the size of the text to 0.8em
* `.text-center` &mdash; center text
* `.text-left` &mdash; align text left
* `.text-right` &mdash; align text right

### grid
* `.clearing` &mdash; clears left-floating `.grid-#` elements
* `.grid-#` &mdash; defines an element spanning `#` columns in the grid
* `.layout` &mdash; defines a layout

Try something like the following to test it out:

	<h1>Greetings from the Northland!</h1>
	<ul class="layout">
		<li class="grid-4">Baffin</li>
		<li class="grid-4">Helluland</li>
		<li class="grid-4">Qikiqtaaluk</li>
	</ul>

Author
------
RJ Zaworski <rj@rjzaworski.com>

License
-------
geous.js is released under the JSON License. You can read the license [here](http://www.json.org/license.html).
