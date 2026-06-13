---
layout: home
---

<div class="hero">
  <div class="hero-eyebrow">South Africa's fitness resource</div>
  <h1 class="hero-headline">Train<br><em>harder.</em><br>Know more.</h1>
  <p class="hero-sub">Workout plans, supplement reviews, and gear guides — built for South African athletes and beginners alike.</p>
  <div class="cta-row">
    <a href="/workouts/" class="cta-primary">Browse workouts</a>
    <span class="cta-secondary">or explore supplements →</span>
  </div>
</div>

<div class="slash-divider"></div>

<div class="featured">
  <div>
    <div class="featured-tag">Featured guide</div>
    <div class="featured-title">PPL - The Split that Suits EVERYONE</div>
    <p class="featured-desc">Learn about PPL and why it suits a busy schedule.</p>
  </div>
  <a href="/nutrition/2026-06-03-ppl-article/" class="featured-badge">Read guide</a>
</div>

<div class="section">
  <div class="section-label">Latest articles</div>
  <div class="cards">
    {% for post in site.posts limit:3 %}
    <a href="{{ post.url | relative_url }}" class="card">
      <span class="card-slash"></span>
      <div class="card-tag">{{ post.categories[0] }}</div>
      <div class="card-title">{{ post.title }}</div>
      <div class="card-meta">{{ post.date | date: "%b %d, %Y" }} &middot; {{ post.read_time | default: "5 min read" }}</div>
    </a>
    {% endfor %}
  </div>
</div>