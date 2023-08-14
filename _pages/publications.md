---
layout: page
permalink: /Publications/
title: Publications
description:
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

# First-author publications
------------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=T] %}

# Co-author publications
--------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=F] %}

</div>
