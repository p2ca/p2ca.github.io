---
layout: page
permalink: /publications/
title: publications
description: peer-reviewed publications in reverse chronological order.
nav: true
nav_order: 1
---

<style>
  /* al-folio gives the thumbnail column 2 of 12 grid columns and the text 8,
     leaving 2 columns of every publication row unused. Reclaim them so the
     preview figure is large enough to read instead of a 125px smudge. */
  .publications .row > .col-sm-2.abbr {
    flex: 0 0 24%;
    max-width: 24%;
  }
</style>

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
