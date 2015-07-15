---
layout: page-people
title: "Search"
permalink: "/search/"
meta_title: "Search Verhaak Lab"
meta_description: "Search Verhaak Lab - Powered by Google Custom Search"
comments: false
show_meta: false
#teaser: SYSTEM GENERATED PAGE FOR SEARCH FUNCTIONS. DO NOT EDIT/RENAME/REMOVE THIS PAGE.
---

<div id="searchbox" align="center">
<div class="searchcont">
    <span class="searchicon"><i class="fa fa-search fa-2x"></i></span>
    <form role="search" method="get" action="{{ site.url }}/cse/">
        <input id="searchString" name="searchString"
               placeholder=" Search Verhaak Lab" type="text">
    </form>
</div>
</div>

<hr>

<a class="list-group-item" href="{{ site.url }}/tags/" title="Keyword based search" alt="Keyword based search"><i class="fa fa-tags fa-1x"></i> Try keyword based search</a>

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="slidetags">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li style="font-size:{{ site.tags[this_word].size | times: 100 | divided_by: site.tags.size | plus: 70 }}%"><a href="{{ site.url }}/tags/#{{ this_word }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

