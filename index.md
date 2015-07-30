---
layout: page-fullwidth
meta_title: "Verhaak Lab at the UT MD Anderson Cancer Center"
meta_description: "Verhaak Lab's research focus is the analysis of cancer genomics data to improve our understanding of cancer biology."
#header:
#    title:
#    background-color: "#EFC94C;"
#    pattern: pattern_concrete.jpg
#    image_fullwidth: unsplash_brooklyn-bridge_header.jpg
#    caption: This is a caption for the header image with link
#    caption_url: https://unsplash.com/
comments: false
show_meta: false
---

We are a computational cancer biology lab at the [UT MD Anderson Cancer Center](http://www.mdanderson.org), Houston, TX. Our lab is affiliated with the [Department of Genomic Medicine](http://www.mdanderson.org/education-and-research/departments-programs-and-labs/departments-and-divisions/genomic-medicine/index.html) and the [Department of Bioinformatics and Computational Biology](http://bioinformatics.mdanderson.org) at UT MD Anderson Cancer Center.  

Our research focus is in the analysis of cancer genomics data to improve our understanding of cancer biology. We have a specialized research interest in understanding disease progression of brain tumors, particularly *glioblastoma and glioma*. We mostly use high throughput sequencing and computational analysis in our research.

### <i class="fa fa-info-circle fa-1.9x"> News</i>

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

### <i class="fa fa-twitter fa-1.9x"> Latest Tweets from the Lab</i>

<ul class="small-block-grid-2">
<li>
<div class="mytweets">
<a class="twitter-timeline"
  data-dnt="true"
  width="600"
  height="250"
  href="https://twitter.com/RoelVerhaak"
  data-widget-id="609868819989815296"
  data-tweet-limit="2"
  data-chrome="noheader nofooter noborders noscrollbar transparent">
  Recent Tweets</a>
</div>
<script>
    !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
</script>
</li>
<li>
<div class="mytweets">
<a class="twitter-timeline"
  data-dnt="true"
  href="https://twitter.com/SBAmin/lists/verhaak-lab" 
  data-widget-id="623382009931436032"
  width="600"
  height="250"
  data-tweet-limit="2"
  data-chrome="noheader nofooter noborders noscrollbar transparent">Tweets from Verhaak Lab</a>
</div>
<script>
    !function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");
</script>
</li>
</ul>

<br>

<ul class="small-block-grid-2">
<li><a href="http://gsbs.uth.edu"><img alt="The University of Texas Graduate School of Biomedical Sciences at Houston" title="The University of Texas Graduate School of Biomedical Sciences at Houston" src="{{ site.url }}/images/logos/utgsbs_logo.png"></a></li>
<li><a href="http://bcm.edu/scbmb"><img alt="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" title="Affiliated with SCBMB Graduate Program at Baylor College of Medicine" src="{{ site.url }}/images/logos/scbmb_bcm_logo.png"></a></li>
</ul>

