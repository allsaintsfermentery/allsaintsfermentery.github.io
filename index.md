---
layout: default
---

> We brew for the greater glory of God and in honor of all His faithful saints.

All Saints Fermentery was established in 2025 to honor the saints who dedicated their lives to God and to enrich Catholic traditions, particularly during feast days, through celebratory beverages.

We take pride in developing each recipe to produce high-quality beers intended for sharing during meals, celebrations, or other significant occasions.

We encourage you to visit this page regularly for updates regarding our brewing schedule and forthcoming releases.

> Omnes Sancti et Sanctae Dei, orate pro nobis.

## Our Beers

{% if site.data.beers %}
{% assign available = site.data.beers | where: "status", "Available" %}
{% assign seasonal = site.data.beers | where: "status", "Seasonal" %}
{% assign coming_soon = site.data.beers | where: "status", "Coming Soon" %}

{% if available.size > 0 %}
### Available Now

| Beer | Style | ABV | Description |
|------|-------|-----|-------------|
{%- for beer in available %}
| **{{ beer.name }}** | {{ beer.style }} | {{ beer.abv }}% | {{ beer.description }} |
{%- endfor %}
{% endif %}

{% if seasonal.size > 0 %}
### Seasonal

| Beer | Style | ABV | Description |
|------|-------|-----|-------------|
{%- for beer in seasonal %}
| **{{ beer.name }}** | {{ beer.style }} | {{ beer.abv }}% | {{ beer.description }} |
{%- endfor %}
{% endif %}

{% if coming_soon.size > 0 %}
### Coming Soon

| Beer | Style | ABV | Description |
|------|-------|-----|-------------|
{%- for beer in coming_soon %}
| **{{ beer.name }}** | {{ beer.style }} | {{ beer.abv }}% | {{ beer.description }} |
{%- endfor %}
{% endif %}

{% else %}
*Our beer list is being updated. Check back soon!*
{% endif %}
