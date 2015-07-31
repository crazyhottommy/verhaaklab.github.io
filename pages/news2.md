---
layout: page
title: "Category: News"
teaser: "Blog posts marked with category: <i>News</i>. For all posts, go to blog"
meta_title: "Category marked with News - Verhaak Lab"
meta_description: "Blog posts marked with category: news. For all posts, go to blog"
#header:
#   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/news2/"
comments: false
show_meta: false
sitemap: false
#teaser: SYSTEM GENERATED PAGE FOR KEYWORDS FUNCTIONS. DO NOT EDIT/RENAME/REMOVE THIS PAGE.
---

<div id="blog-index" class="row">
  <div class="small-12 columns t30">
    <dl class="accordion" data-accordion>
      {% assign counter = 1 %}
      {% for post in site.categories.news limit:5 %}
      <dd class="accordion-navigation">
      <a href="#panel{{ counter }}"><span class="iconfont"></span> {% if post.date %}<time class="icon-calendar pr20" datetime="{{ post.date | date: "%Y-%m-%d" }}" itemprop="datePublished"> {{ post.date | date: "%Y-%m-%d" }}</time> {% endif %}<strong>{{ post.title }}</strong></a>
        <div id="panel{{ counter }}" class="content">
          {% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}
          <a href="{{ site.url }}{{ post.url }}" title="Read {{ post.title escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a><br><br>
        </div>
  </dd>
      {% assign counter=counter | plus:1 %}
      {% endfor %}
  </dl>
</div><!-- /.small-12.columns -->
</div><!-- /.row -->
<br>

### Other Categories:

<ul class="tags-ts">
    {% for category in site.categories | sort %}
        <li style="font-size:{{ category | last | size | times: 100 | divided_by: site.categories.size | plus: 80 }}%">
            <a class="tag-ts" href="{{ site.url }}/{{ category | first | slugize }}/">
                {{ category | first }}
            </a>
        </li>
    {% endfor %}
</ul>

### [Archived posts with tag *news*]({{ site.url }}/tags/#news)


