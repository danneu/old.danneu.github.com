---
layout: post
title: "Darkstrap.css: A Dark Theme for Twitter Bootstrap 2"
permalink: "posts/4-darkstrap-css-a-dark-theme-for-twitter-bootstrap-2"
---

**Update (27th Jan 2013):** Darkstrap v0.9.0 released. Compatible with Twitter Bootstrap v2.2.2.

* New [Darkstrap vs. Bootstrap demo][demo].
* More info on the [Github page][github].

I'm still ironing out some cross-browser issues (but it's still better than the original darkstrap.css).

It's also when I decided to start versioning it at v0.9.0. I'd like v1.0 to be a solid release across browsers.

I'm also unsure of some decision decisions which I'd like to stabilize for v1.0.

----

A couple days ago, [Mark Otto][otto] and [Jacob Thorton][thorton] released [Twitter Bootstrap 2.0][bootstrap], the latest version of their popular html/css/js toolkit. It's nice and clean... and very white.

I'm working on a project that demands a darker theme, so I made `darkstrap.css` that turns the lights out on Bootstrap vanilla. Just include it after the Bootstrap stylesheet so it can cascade over the lighter theme.

~~~ html
<link href='stylesheets/darkstrap.css' rel='stylesheet' />
~~~

Simple as.

# Check it out

* Demo: [Darkstrap vs. Bootstrap][demo]
* Download [darkstrap.css][css]
* Darkstrap on [Github][github] 

![Comparison of Bootstrap and Darkstrap colors][comparison]

# Legacy Darkstrap

I preserved the original darkstrap.css if anybody needs it for whatever reason.

* [Original demo][dark-demo]
* [Original darkstrap.css file][legacycss]

[otto]: http://twitter.com/mdo
[thorton]: http://twitter.com/fat
[bootstrap]: http://twitter.github.com/bootstrap/
[comparison]: /bag/darkstrap/images/comparison.png "Bootstrap Vanilla vs Darkstrap"
[github]: https://github.com/danneu/darkstrap
[css]: /bag/darkstrap/css/darkstrap-v0.9.0.css
[legacycss]: /bag/darkstrap/legacy/stylesheets/darkstrap.css
[dark-demo]: /bag/darkstrap/legacy/darkstrap.html
[vanilla-demo]: /bag/darkstrap/legacy/bootstrap.html
[swatch]: http://bootswatch.com/ 
[demo]: /bag/darkstrap/darkstrap.html
[github]: https://github.com/danneu/darkstrap 
