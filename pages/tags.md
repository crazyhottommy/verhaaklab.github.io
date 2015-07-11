---
layout: page
title: "Search By Categories / Tags"
permalink: "/tags/"
meta_title: "Keyword based search - Verhaak Lab"
meta_description: "Browse Verhaak Lab by category and tag based index"
comments: false
show_meta: false
sitemap: true
#teaser: SYSTEM GENERATED PAGE FOR KEYWORDS FUNCTIONS. DO NOT EDIT/RENAME/REMOVE THIS PAGE.
---

<ul class="tags-ts">
    {% for category in site.categories | sort %}
        <li style="font-size:{{ category | last | size | times: 100 | divided_by: site.categories.size | plus: 80 }}%">
            <a class="tag-ts" href="/{{ category | first | slugize }}/">
                {{ category | first }}
            </a>
        </li>
    {% endfor %}
</ul>

<hr>

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="tag-box inline">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li style="font-size:{{ site.tags[this_word].size | times: 100 | divided_by: site.tags.size | plus: 90 }}%"><a href="#{{ this_word }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

{% for item in (0..site.tags.size) %}{% unless forloop.last %}
  {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
<h2 id="{{ this_word }}">{{ this_word }}</h2>
<ul class="post-list">
  {% for post in site.tags[this_word] %}{% if post.title != null %}
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %d, %Y" }}</time></span></a></li>
  {% endif %}{% endfor %}
  </ul>
{% endunless %}{% endfor %}

<br>




