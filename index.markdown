---
layout: home
---

<div class="parallax-hero">
  <div class="parallax-overlay"></div>
  <div class="parallax-content">
    <div class="hero-eyebrow">South Africa's fitness resource</div>
    <h1 class="hero-headline">Train<br><em>harder.</em><br>Know more.</h1>
    <p class="hero-sub">For Anything and Everything Gym — built for South African athletes and beginners alike.</p>
    <div class="cta-row">
      <a href="{{ '/workouts/' | relative_url }}" class="cta-primary">Browse workouts and fitness articles</a>
    </div>
  </div>
</div>

<div class="slash-divider"></div>

<div class="featured">
  <div>
    <div class="featured-tag">Featured guide</div>
    <div class="featured-title">PPL - The Split that Suits EVERYONE</div>
    <p class="featured-desc">Learn about PPL and why it suits a busy schedule.</p>
  </div>
 <a href="{{'/workouts/ppl-article/' | relative_url }}" class="featured-badge">Read guide</a>
</div>

<div class="section">
  <div class="section-label">Latest articles</div>
  <div class="cards">
    {% for post in site.posts limit:3 %}
    <a href="{{ post.url | relative_url }}" class="card">
      {% if post.image %}
      <div class="card-image" style="background-image: url('{{ post.image }}')"></div>
      {% endif %}
      <span class="card-slash"></span>
      <div class="card-tag">{{ post.categories[0] }}</div>
      <div class="card-title">{{ post.title }}</div>
      <div class="card-meta">{{ post.date | date: "%b %d, %Y" }}</div>
    </a>
    {% endfor %}
  </div>
</div>