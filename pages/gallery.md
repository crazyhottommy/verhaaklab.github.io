---
layout: page-people
title:  "Group Photos"
meta_title: "Photo Gallery - Verhaak Lab"
meta_description: "Pictures of Lab  and other events"
#teaser: ""
categories:
    - people
tags:
    - members
    - photos
    - pictures
    - outing
    - picnic
    - retreat
permalink: "/people/gallery/"
comments: false
show_meta: false
breadcrumb: true
gallery:
    - June-2013: /retreat/verhaaklab-20130617.jpg
    - May-2012: /retreat/groupphoto.201205.png
    - April-2012: /retreat/groupphoto.201204.png
#   - Caption:  /path_to_picture_inside_images_dir.jpg
---

<ul class="clearing-thumbs small-block-grid-3" data-clearing>
{% for link_hash in page.gallery %}
  {% for link in link_hash %}
    <li><a href="{{ site.urlimg }}{{ link[1] }}" title="{{ link[0] }}"><img  data-caption="{{ link[0] }}" class="th" src="{{ site.urlimg }}{{ link[1] }}" alt="{{ link[0] }}"></a></li>
  {% endfor %}
{% endfor %}
</ul>

### [Picasa Gallery](http://bit.ly/verhaklab_pics)
