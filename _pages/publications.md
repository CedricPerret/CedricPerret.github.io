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

<h1>First-authored publications</h1>
------------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=T] %}

<h1>Co-authored publications</h1>
--------------------

{% bibliography -f {{ site.scholar.bibliography }} --query @*[note=F] %}

</div>
