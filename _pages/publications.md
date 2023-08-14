---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

The default Bibliography
------------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=T] %}

Secondary References
--------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=F] %}

</div>
