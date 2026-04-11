---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<style>
.pub-card {
  border-left: 4px solid #3a9e70;
  padding: 1.1em 1.4em 1em 1.4em;
  margin-bottom: 1.4em;
  background: #f8fafb;
  border-radius: 0 6px 6px 0;
  box-shadow: 0 1px 3px rgba(0,0,0,0.06);
  transition: box-shadow 0.15s ease, border-left-color 0.15s ease;
}

.pub-card:hover {
  box-shadow: 0 3px 10px rgba(0,0,0,0.11);
  border-left-color: #2d8560;
}

.pub-card__title {
  font-size: 1.05em;
  font-weight: 700;
  margin: 0 0 0.35em 0;
  border-bottom: none !important;
  color: #2a2a2a;
  line-height: 1.35;
}

.pub-card__authors {
  font-size: 0.88em;
  color: #555;
  margin: 0 0 0.25em 0;
}

.pub-card__me {
  font-weight: 700;
  color: #333;
  text-decoration: underline;
  text-underline-offset: 2px;
}

.pub-card__venue {
  font-size: 0.85em;
  color: #666;
  margin: 0 0 0.6em 0;
  font-style: italic;
}

.pub-card__venue a {
  font-style: normal;
  font-weight: 600;
  color: #3a7fbf;
  text-decoration: none;
}

.pub-card__venue a:hover {
  text-decoration: underline;
}

.pub-card__footer {
  display: flex;
  align-items: center;
  gap: 0.5em;
  flex-wrap: wrap;
}

.pub-card__badge--award {
  display: inline-block;
  background: #e8a020;
  color: #fff;
  padding: 2px 9px;
  border-radius: 3px;
  font-size: 0.77em;
  font-weight: 600;
  letter-spacing: 0.01em;
}

.pub-card__link {
  display: inline-block;
  background: #3a9e70;
  color: #fff !important;
  padding: 2px 10px;
  border-radius: 3px;
  font-size: 0.77em;
  font-weight: 600;
  text-decoration: none !important;
  letter-spacing: 0.01em;
  transition: background 0.15s ease;
}

.pub-card__link:hover {
  background: #2d8560;
  color: #fff !important;
}

.pub-card--working .pub-card__link {
  background: #d4823a;
}

.pub-card--working .pub-card__link:hover {
  background: #b86d2e;
}

.page__title {
  display: none;
}

.pub-section-heading {
  font-size: 1.55em;
  font-weight: 800;
  color: #1a1a1a;
  margin: 2.2em 0 1em 0;
  padding: 0.15em 0 0.15em 0.65em;
  border-left: 5px solid #ccc;
  border-bottom: none;
  letter-spacing: -0.01em;
}

.pub-section-heading:first-child {
  margin-top: 0.5em;
}

.pub-section-heading--conference {
  border-left-color: #3a9e70;
}

.pub-section-heading--working {
  border-left-color: #d4823a;
}

/* Expandable cards */
details.pub-card {
  cursor: pointer;
}

details.pub-card > summary {
  list-style: none;
  display: block;
}

details.pub-card > summary::-webkit-details-marker {
  display: none;
}

details.pub-card > summary::marker {
  display: none;
}

.pub-card__chevron {
  font-size: 0.6em;
  color: #aaa;
  vertical-align: middle;
  margin-left: 0.4em;
  transition: transform 0.2s ease;
  display: inline-block;
}

details.pub-card[open] .pub-card__chevron {
  transform: rotate(180deg);
}

.pub-abstract {
  border-top: 1px solid #dde3e8;
  margin-top: 0.8em;
  padding-top: 0.8em;
}

.pub-abstract p {
  font-size: 0.85em;
  color: #555;
  line-height: 1.65;
  margin: 0;
}

.pub-card--working {
  border-left-color: #d4823a;
}

.pub-card--working:hover {
  border-left-color: #b86d2e;
}

.pub-card__badge--preprint {
  display: inline-block;
  background: #d4823a;
  color: #fff;
  padding: 2px 9px;
  border-radius: 3px;
  font-size: 0.77em;
  font-weight: 600;
  letter-spacing: 0.01em;
}
</style>

<h2 class="pub-section-heading pub-section-heading--working">Working Papers</h2>

{% assign working_papers = site.publications | where: "status", "working" | sort: "date" | reverse %}
{% for post in working_papers %}
  {% include pub-single.html %}
{% endfor %}

<h2 class="pub-section-heading pub-section-heading--conference">Conference Papers</h2>

{% assign conference_papers = site.publications | where: "status", "conference" | sort: "date" | reverse %}
{% for post in conference_papers %}
  {% include pub-single.html %}
{% endfor %}
