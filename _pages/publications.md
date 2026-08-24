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
  /* The architecture figure is 2.5:1; in al-folio's narrow thumbnail column it
     renders ~190px wide, which puts its labels at ~3px. Give the preview the
     full row width so the complete figure stays readable, and keep the venue
     badge from stretching along with it. */
  .publications .row > .col-sm-2.abbr {
    flex: 0 0 100%;
    max-width: 100%;
  }
  .publications .row > .col-sm-2.abbr abbr.badge {
    max-width: 150px;
  }
  .publications .row > .col-sm-2.abbr figure {
    margin: 0.6rem 0 0.2rem;
  }
</style>

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
