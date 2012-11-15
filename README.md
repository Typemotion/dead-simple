Dead Simple
===

This is an example template for building templates against the TypeMotion rendering engine.  

The template syntax is based on [Jinja2](http://jinja.pocoo.org/), and should be extremely simple 
in comparison to more all-inclusive templated blogs (Wordpress, et al). 

Static media must be placed in the '/static/' folder, and convention dictates that stylesheets go
into /static/css/, images go into /static/img/ and JavaScript files go into /static/js/.  This isn't
a hard requirement, but will make transitioning from theme to theme all the easier if followed.

Beyond that, all templates extend the "base.html" template, which includes the header, footer and 
everything in between.  This again can be changed, but shouldn't need to be for most templates. 

The default template, which gets compiled into "index.html" at the root of a Typemotion blog, is 
found in the "home.html" template, while the list of archived posts is "archive.html" and individual
blog posts will be found in "detail.html".  "Recent.html" is a convenience page is not strictly 
necessary at all, but providing it speeds template parsing slightly.  It may be omitted if desired, 
but should not be added to the base template directly as that means it would have to parse every 
page in a blog to render it, which should not be necessary on archival pages and others. 
