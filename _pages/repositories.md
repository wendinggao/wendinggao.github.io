---
layout: page
permalink: /repositories/
title: repositories
description: GitHub profile and repositories of Wending Gao.
nav: true
nav_order: 3
---

{% if site.data.repositories.github_users %}
## GitHub users

{% for user in site.data.repositories.github_users %}
{% include repository/repo_user.liquid username=user %}
{% endfor %}

---
{% endif %}

{% if site.data.repositories.github_repos %}
## GitHub Repositories

{% for repo in site.data.repositories.github_repos %}
{% include repository/repo.liquid repository=repo %}
{% endfor %}
{% endif %}
