---
layout: post
title: "Darkstrap.css: A Dark Theme for Twitter Bootstrap 2"
permalink: "posts/4-darkstrap-css-a-dark-theme-for-twitter-bootstrap-2"
---

**Update (27th Jan 2013):** I'm about to release Darkstrap v2.0 which is compatible with the latest Twitter Bootstrap. See more on the [project's README](https://github.com/danneu/darkstrap). 

I'm first ironing out some cross-browser issues.

----

A couple days ago, [Mark Otto][otto] and [Jacob Thorton][thorton] released [Twitter Bootstrap 2.0][bootstrap], the latest version of their popular html/css/js toolkit. It's nice and clean... and very white.

I'm working on a project that demands a darker theme, so I made `darkstrap.css` that turns the lights out on Bootstrap vanilla. Just include it after the Bootstrap stylesheet so it can cascade over the lighter theme.

~~~ html
<link href='stylesheets/darkstrap.css' rel='stylesheet' />
~~~

Simple as.

* [Live demo][dark-demo] vs [Bootstrap demo][vanilla-demo]
* Download [darkstrap.css][css]
* Darkstrap on [Github][github]

## Comparison

![Comparison of Bootstrap and Darkstrap colors][comparison]

I took a lot of the look directly from Compass.

[otto]: http://twitter.com/mdo
[thorton]: http://twitter.com/fat
[bootstrap]: http://markdotto.com/bs2/docs/index.html
[comparison]: /bag/darkstrap/images/comparison.png "Bootstrap Vanilla vs Darkstrap"
[github]: https://github.com/danneu/darkstrap
[css]: https://raw.github.com/danneu/darkstrap/master/stylesheets/darkstrap.css
[legacycss]: /bag/darkstrap/darkstrap_legacy.css
[dark-demo]: /bag/darkstrap/legacy/darkstrap.html
[vanilla-demo]: /bag/darkstrap/legacy/bootstrap.html
[swatch]: http://bootswatch.com/ 
