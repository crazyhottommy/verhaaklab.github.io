---
layout: page
title: "Publications"
meta_title: "Publications - Verhaak Lab"
meta_description: "List of selected and current publications, includes PubMed and Google Scholar listing"
permalink: "/publications/"
header:
#   image_fullwidth: "publpics/wordle_verhaak.png"
comments: false
show_meta: false
---

<div class="panel radius" markdown="1">
{: #toc }
*  TOC
{:toc}
</div>

#### Recent Publications:

<div id="blog-index" class="row">
  <div class="small-12 columns t30">
    <dl class="accordion" data-accordion>
      {% assign counter = 1 %}
      {% for post in site.categories.publication limit:5 %}
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

#### Selected Publications:
***
*   Cancer Genome Atlas Research Network, Brat DJ, Verhaak RG, Aldape KD, et al. Comprehensive, Integrative Genomic Analysis of Diffuse Lower-Grade Gliomas. New England Journal of Medicine; 2015. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/26061751)

*   Kim H, Zheng S, .., Verhaak RG. Whole-genome and multisector exome sequencing of primary and post-treatment glioblastoma reveals patterns of tumor evolution. Genome Res; 2015. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/25650244)
 
*   Zheng S, Kim H, Verhaak RG. Silent mutations make some noise. Cell; 2014. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/24630716)
 
*   Yoshihara K, Shahmoradgoli M, .., Verhaak RG. Inferring tumour purity and stromal and immune cell admixture from expression data. Nature Communications; 2013. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/24113773)

*   Brennan C, Verhaak RG, McKenna A, et al. The Somatic Genomic Landscape of Glioblastoma. Cell; 2013. [Abstract](http://t.co/2kt3f2hu3I)

*   Zheng S, Fu J, .., Verhaak RG. A survey of intragenic breakpoints in glioblastoma identifies a distinct subset associated with poor survival. Genes Dev; 2013. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/23796897)

*   Verhaak RG, Tamayo P, Yang JY, et al. Prognostically relevant gene signatures of high-grade serous ovarian carcinoma. J Clin Invest; 2013. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/23257362)

*   Verhaak RG, et al. Integrated genomic analysis identifies clinically relevant subtypes of glioblastoma characterized by abnormalities in PDGFRA, IDH1, EGFR, and NF1. Cancer Cell; 2010.  [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/20129251)

*   Verhaak RG, et al. Mutations in nucleophosmin (NPM1) in acute myeloid leukemia (AML). Blood; 2005. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/16109776)

*   Valk PJ, Verhaak RG, Beijen MA, et al. Prognostically useful gene-expression profiles in acute myeloid leukemia. New England Journal of Medicine; 2004. [Abstract](http://www.ncbi.nlm.nih.gov/pubmed/15084694)

***

#### [Citations at Google Scholar](http://scholar.google.com/citations?user=qXdBk-gAAAAJ&hl=en)

#### [PubMed Listing](http://www.ncbi.nlm.nih.gov/pubmed?term=verhaak+r)
