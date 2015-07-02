---
layout: page-people
title: Custom Search
permalink: "/cse/"
sitemap: false
noindex: true
comments: false
show_meta: false
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
<script>
        (function() {
            var cx = '{{site.google_search}}';
            var gcse = document.createElement('script');
            gcse.type = 'text/javascript';
            gcse.async = true;
            gcse.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') +
            '//www.google.com/cse/cse.js?cx=' + cx;
            var s = document.getElementsByTagName('script')[0];
            s.parentNode.insertBefore(gcse, s);
        })();
</script>
<gcse:searchresults-only queryParameterName="searchString"></gcse:searchresults-only>
<hr>
<div id="searchbox" align="center">
<div class="searchcont">
    <span class="searchicon"><i class="fa fa-search fa-2x"></i></span>
    <form role="search" method="get" action="{{ site.url }}/cse/">
        <input id="searchString" name="searchString"
               placeholder=" Search Verhaak Lab" type="text">
    </form>
</div>
</div>

