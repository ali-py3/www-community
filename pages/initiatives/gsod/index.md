---

layout: col-sidebar
title: Google Season of Docs
tags: gsod, Google Season of Docs
permalink: /initiatives/gsod/

---

## Information

OWASP was part of the initial Google Season of Docs last year

[GSoC Student Application Template (SAT)](gsoc_sat)

### Current
{% assign current = site.pages | where: 'url', '/initiatives/gsod/current/' | first %}
* [{{current.title}}]({{current.url}})

### Historical
{% assign pages = site.pages | sort: 'title' | where_exp: "page", "page.path contains 'gsod/historical'" | where_exp: "page", "page.name != 'info.md'" %}
{% for historical in pages %}
* [{{historical.title}}]({{historical.url}})
{% endfor %} 