Jekyll Template Toolkit (JTT)
=============================

A widget collection for vanilla jekyll, 100% compatible to github-pages.

All widgets work in a vanilla jekyll installation, ensuring that a site that is built with these 
templates can also sucessfully be built on GitHub. This makes JTT a very useful toolkit for the use
with GitHub Pages.

You can confirm this locally by running
	
		jekyll --safe

Each widget is a self-contained piece of code that can simply be included via 

		{% include widgets/widget.html %}. 
	
There are also some predefined boilerplate pages and layouts that make the day-to-day work with 
jekyll much easier. feel free to use and adapt them for your own blog.

The HTML markup used in all files is HTML5. I tried to use it as semantically correct as possible.
If you find any mistakes, please open an issue or fork & submit a pull request as fix.
		
	
Getting started
---------------

You can copy-paste everything you need from the repo, but the recommended way is to clone the repo via

		git clone git://github.com/NetzwergX/jekyll-template-toolkit.git


Widgets
-------

Widgets are located inside the `_includes/widgets/` folder.

* **Category List** (categoryList.html)
	A simple list containing all categories and the number of posts in them.
	Useful for navigations e.g. in sidebars.

* **Post Timeline** (timeLine.html)
	A time line containing all month in which posts were published, grouped by year.
	Useful for navigations e.g. in sidebars.

* **Tag Cloud** (tagCloud.html)
	A linear weighted tag cloud. 
	
* **Similar posts list** (similarPostList.html)
	A list containing similar posts.
	Useful to provide some "Further reading" links to the user. Only works on post pages.
	
* **Google Search box** (googleSearchForm.html)
	A very simple search box with an input field and submit button. searches via google.
	TODO: Add JS-support to add site:my.domain to the query.
		
Planned widgets (WIP)
	
* **Tapir search box**
	A search box for searching the site via Tapir (<http://tapirgo.com/>).	
		
Pages
-----

Pages are located directly inside the root folder.

* **Category Page** (categories.html)
	A page listing all posts grouped by category.
	Has IDs in order to jump to a specific category directly.

* **Archive Page** (archive.html)
	A page listing all posts grouped by year and month.
	Has IDs in order to jump to a specif month or month-year combination directly.

* **Full Feed Page** (fullFeed.xml)
	Provides an RSS 2.0 Feed containing all posts.	
	
* **Feed Page** (fullFeed.xml)
	Provides an RSS 2.0 Feed containing the X latest posts. Defaults to 5.	
		
Layouts
-------

Layout are located inside the `_layouts/` folder.

* **Page** (page.html)
	Boilerplate base layout for all layouts.
	
* **Index** (index.html)
	Index page rendering post list with pagination.
	
* **Article** (article.html)
	Post page showing one post.
	
* **Feed** (feed.xml)
	Base layout for RSS 2.0 feeds.
		
	
Contribution (Code of conduct)
------------------------------

**Contribution is highly encouraged**. If you think you found a great piece code that is useful
for jekyll users, feel free to contribute!

There are some rules though:
	
* Do not spam-commit. Use a sensible # of commits.
* Split logical changes into separate commits, avoid gigantic commits.
* Write meaningful commit messages
* Avoid lines with more then 100 characters wherever possible.
* Use **tabs** for indentation, spaces for alignment.
* Do not harm anyone while using or contributing to this software
		
More information
----------------

Updates on JTT and articles about blogging on github-pages can be found regularly
[on my blog at teumert.net](http://www.teumert.net/).

		
License
-------
(The MIT License)

Copyright (c) 2012 Sebastian Teumert (<http://www.teumert.net>, <http://github.com/NetzwergX>)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the 'Software'), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.