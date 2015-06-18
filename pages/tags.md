---
layout: page
title: "Tags"
teaser: "Browse website by keywords"
permalink: "/tags/"
comments: false
show_meta: false
---

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="tag-box inline">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ this_word }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

{% for item in (0..site.tags.size) %}{% unless forloop.last %}
  {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
<h2 id="{{ this_word }}">{{ this_word }}</h2>
<ul class="post-list">
  {% for post in site.tags[this_word] %}{% if post.title != null %}
  <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></li>
  {% endif %}{% endfor %}
  </ul>
{% endunless %}{% endfor %}

<br>

### Category wise search:

<ul class="tags-ts">
    {% for category in site.categories | sort %}
        <li style="font-size:{{ category | last | size | times: 100 | divided_by: site.categories.size | plus: 80 }}%">
            <a class="tag-ts" href="/{{ category | first | slugize }}/">
                {{ category | first }}
            </a>
        </li>
    {% endfor %}
</ul>


