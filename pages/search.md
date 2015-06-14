---
layout: page
show_meta: false
title: "Search"
permalink: "/search/"
---

{% include google_search.html %}

<form style="padding-bottom: 200px;" onsubmit="google_search()" >
  <input type="text" id="google-search" placeholder="{{ site.data.language.enter_search_term }}">
</form>

#### Can't find what you're looking for?

<a class="list-group-item" href="https://twitter.com/roelverhaak" title="Follow me @roelverhaak" alt="Follow me @roelverhaak"><i class="fa fa-twitter fa-2x"></i></a> &nbsp;&nbsp;&nbsp;&nbsp; <a class="list-group-item" href="http://verhaaklab.github.io/feed.xml" title="Updates via RSS feed" alt="Updates via RSS feed"><i class="fa fa-rss fa-2x"></i></a>  &nbsp;&nbsp;&nbsp;&nbsp; <a class="list-group-item" href="{{ site.url }}/contact/" title="Contact Us" alt="Contact Us"><i class="fa fa-envelope fa-2x"></i></a>

