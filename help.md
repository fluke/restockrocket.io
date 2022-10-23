---
title: Help Center
list_title: 'Help Center'
url: '/help'
layout: home
image:
  path: '/assets/img/Banner.png'
  alt: Restock Rocket notifies customers when products are back in stock
---
<h1 class="page-heading">Help Center<br/></h1>
{% for category in site.categories %}
  <div class="category-container">
    <h3>{{ category[0] }}</h3>
    <div class="posts-container">
      {% for post in category[1] %}
        <div class="single-post">
          <h4><a class="help-center-link" href="{{ post.url }}">{{ post.title }}</a></h4>
          <p class="teaser">{{post.teaser}}</p>
        </div>
      {% endfor %}
    </div>
  </div>
{% endfor %}
