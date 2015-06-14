---
layout: page-fullwidth
title: ""
subheadline: ""
#teaser: "Verhaak Lab at the UT MD Anderson Cancer Center"
categories:
    - design
tags:
    - design
#header:
#    title:
#    background-color: "#EFC94C;"
#    pattern: pattern_concrete.jpg
#    image_fullwidth: unsplash_brooklyn-bridge_header.jpg
#    caption: This is a caption for the header image with link
#    caption_url: https://unsplash.com/
---
## Welcome to Verhaak Lab

>This is a beta and unofficial version for a potential new look of our lab website. For current and most up-to-date version, please visit official website, **[http://odin.mdacc.tmc.edu/~rverhaak](http://odin.mdacc.tmc.edu/~rverhaak)**

We are a computational cancer biology lab at the [UT MD Anderson Cancer Center](http://www.mdanderson.org), Houston, TX. Our lab is affiliated with Department of Genomic Medicine and [Department of Bioinformatics and Computational Biology](http://bioinformatics.mdanderson.org) at the MD Anderson Cancer Center.


### <center><i class="fa fa-info-circle fa-1.9x"></i> Recent News</center>

<div id="blog-index" class="row">
  <div class="small-12 columns t30">
    <dl class="accordion" data-accordion>
      {% assign counter = 1 %}
      {% for post in site.posts limit:5 %}
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

<center>
<div class="mytweets">
<a class="twitter-timeline"
  width="600"
  height="250"
  href="https://twitter.com/RoelVerhaak"
  data-widget-id="609868819989815296"
  data-chrome="nofooter noborders transparent">
</a></a>
</div>
<script>
    !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
</script>
</center>

<br>

<ul class="small-block-grid-2">
<li><a href="http://gsbs.uth.edu"><img alt="The University of Texas Graduate School of Biomedical Sciences at Houston" title="The University of Texas Graduate School of Biomedical Sciences at Houston" src="{{ site.url }}/images/logos/utgsbs_logo.png"></a></li>
<li><a href="http://bcm.edu/scbmb"><img alt="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" title="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" src="{{ site.url }}/images/logos/scbmb_bcm_logo.png"></a></li>
</ul>

