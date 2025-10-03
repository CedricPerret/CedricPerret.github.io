---
layout: page
permalink: /repositories/
title: Repositories
description: 
nav: true
nav_order: 3
---

# Featured Repository

Over the years I accumulated code building different evolutionary models.  I decided to bring it all together into a clean Julia package for reusability and to make it useful for other researchers.  Go check it out! (All details are in the README.)

**[JuliassicPark.jl](https://github.com/CedricPerret/JuliassicPark)** – a Julia package for simulating evolutionary models with customizable fitness functions, mutation, and reproduction schemes.  

---

## GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  {% if site.data.repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %}

---

Here are a few of my other GitHub repositories.  
They mostly serve as archives for the code I used in past publications.  

If you are interested in re-using or extending this work, I strongly recommend using **[JuliassicPark.jl](https://github.com/CedricPerret/JuliassicPark.jl)** instead.  
It is much cleaner, faster, and actively maintained.  

Feel free to contact me if you need help!

---
## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
