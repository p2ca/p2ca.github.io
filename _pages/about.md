---
layout: about
title: about
permalink: /
subtitle: M.S. student in Electrical Engineering, <a href='https://www.nyu.edu/'>New York University</a>

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Dept. of Electrical and Computer Engineering</p>
    <p>New York University</p>
    <p>New York, NY</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---


<style>
  /* Headshot is a tight ID-photo crop, so render it smaller than the
     al-folio default width; more-info text wraps under it. */
  .profile {
    max-width: 200px;
  }
  .profile img {
    width: 100%;
    height: auto;
  }
  /* al-folio bolds only the given name by default; bold the surname to match. */
  .post-title {
    font-weight: var(--font-weight-bold, 700);
  }
</style>

I am an M.S. student in Electrical Engineering at **New York University**, where I work on machine learning
under distribution shift. Before NYU I received my B.Eng. in Automation from **Tsinghua University**.

My research asks a fairly practical question: **when we transfer a learned model to a new environment, what
should actually transfer, and what should not?** Most transfer methods align source and target
representations wholesale, which quietly forces genuinely site-specific structure to be shared. I am more
interested in *decomposing* a representation into the part that generalizes and the part that does not, so
that both can be used deliberately.

I currently work on this in the context of **hydrological forecasting**. In collaboration with researchers at
Oak Ridge National Laboratory and Stevens Institute of Technology, I developed DARSD-ResMetaLSTM, which
decomposes latent states with a learnable invariant basis to forecast inflow at data-scarce reservoirs.
Evaluated across six snow/rain transfer scenarios on 33 U.S. reservoirs, it outperforms standard alignment
baselines in both cross-regime directions.

Earlier, at Tsinghua's Institute of Information Processing, I worked on **camouflaged and salient object
detection**, studying how objects that are visually entangled with their background can still be separated —
in retrospect, a computer-vision version of the same decomposition question.

I am applying to **Ph.D. programs for Fall 2027**. If my work overlaps with yours, I would be glad to hear
from you.
