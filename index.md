---
layout: page-fullwidth
title: ""
subheadline: ""
#teaser: "Verhaak Lab at the UT MD Anderson Cancer Center"
categories:
    - design
tags:
    - design
    - background color
    - header
#header:
#    title:
#    background-color: "#EFC94C;"
#    pattern: pattern_concrete.jpg
#    image_fullwidth: unsplash_brooklyn-bridge_header.jpg
#    caption: This is a caption for the header image with link
#    caption_url: https://unsplash.com/
---

## Welcome to Verhaak Lab
<br>
We are a computational cancer biology lab at the [UT MD Anderson Cancer Center](http://www.mdanderson.org), Houston, TX. Our lab is affiliated with Department of Genomic Medicine and [Department of Bioinformatics and Computational Biology](http://bioinformatics.mdanderson.org) at the MD Anderson Cancer Center. We are supported by [NIH][1]. 


### Recent News:

<div id="blog-index" class="row">
  <div class="small-12 columns t30">
    <dl class="accordion" data-accordion>
      {% assign counter = 1 %}
      {% for post in site.posts limit:5 %}
      <dd class="accordion-navigation">
      <a href="#panel{{ counter }}"><span class="iconfont"></span> {% if post.subheadline %}{{ post.subheadline }} › {% endif %}<strong>{{ post.title }}</strong></a>
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


[1]: http://projectreporter.nih.gov/Reporter_Viewsh.cfm?sl=13EDC0034F8FC6D27598B8961CAA4A01A2FFCEB861BF
