---
layout: page
title: "Education"
teaser: "Research Opportunities"
meta_title: "Research Positions - Verhaak Lab"
meta_description: "Academic training opportunities for motivated and talented postdoctoral candidates, graduate students and summer rotation students in areas of cancer computational biology in Verhaak Lab at the UT MD Anderson Cancer Center, Houston, TX"
#header:
#   image_fullwidth: "header_roadmap_3.jpg"
permalink: "/positions/"
comments: false
show_meta: false
---

We are always open to  motivated and talented postdoctoral candidates, graduate students and summer rotation students in areas of computational biology,   and medicine or molecular biology applicants with an interest in computational biology. 

For questions regarding available training opportunities, please [contact Roel]({{ site.url }}/contact/).

For graduate research training, we are  affiliated with the [UT MD Anderson Cancer Center GSBS Program](http://gsbs.uth.edu) and the [SCBMB Graduate Program at Baylor College of Medicine](http://bcm.edu/scbmb).

<ul class="small-block-grid-2">
<li><a href="http://gsbs.uth.edu"><img alt="The University of Texas Graduate School of Biomedical Sciences at Houston" title="The University of Texas Graduate School of Biomedical Sciences at Houston" src="{{ site.url }}/images/logos/utgsbs_logo.png"></a></li>
<li><a href="http://bcm.edu/scbmb"><img alt="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" title="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" src="{{ site.url }}/images/logos/scbmb_bcm_logo.png"></a></li>
</ul>

### <center><i class="fa fa-info-circle fa-1.9x"></i> Latest Posts: Open Positions

<div id="blog-index" class="row">
  <div class="small-12 columns t30">
    <dl class="accordion" data-accordion>
      {% assign counter = 1 %}
      {% for post in site.categories.position limit:5 %}
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

### [Archived posts with tag: *positions*]({{ site.url }}/tags/#positions) 
