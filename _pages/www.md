---
layout: blog
permalink: /www/
title: What Will We
nav: false
heading: What Will We
---


<br>

 <div class="header-bar">
 
    <h2>What Will We</h2>
  </div>

<br>

What Will We… do the same? Or perhaps change? 

 
Since early 2020 scientists across the world begun changing the way they approach research activities: these changes have continued to fluctuate and are now slowly converging into what we will likely call our <i>new normal</i>, a quasi stable point in which we find ourselves comfortable having rediscovered our boundaries and strengths.  

In this series of interviews with mathematicians (and scientists) from around the world, we look at what habits they have developed in the last years which they will nurture in the future, and which activities they think will no longer deserve their time or attention. We will learn from each other with hopes of making our academic life each day more enjoyable and stimulating, and at the same time give a glimpse of why each of us wakes up every morning wanting do do science. 
  

 
 

  <ul class="post-list">
    {% for post in paginator.posts %}

    {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
    {% assign year = post.date | date: "%Y" %}
    {% assign tags = post.tags | join: "" %}
    {% assign categories = post.categories | join: "" %}

    <li>
      <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h3>
      <p>{{ post.description }}</p>
      <p class="post-meta"> {{read_time}} min read &nbsp; &middot; &nbsp;
        {{ post.date | date: '%B %-d, %Y' }}
      </p>
      <p class="post-tags">
        <a href="{{ year | prepend: '/blog/' | prepend: site.baseurl}}">
          <i class="fas fa-calendar fa-sm"></i> {{ year }} </a>

          {% if tags != "" %}
          &nbsp; &middot; &nbsp;
            {% for tag in post.tags %}
            <a href="{{ tag | prepend: '/blog/tag/' | prepend: site.baseurl}}">
              <i class="fas fa-hashtag fa-sm"></i> {{ tag }}</a> &nbsp;
              {% endfor %}
          {% endif %}

          {% if categories != "" %}
          &nbsp; &middot; &nbsp;
            {% for category in post.categories %}
            <a href="{{ category | prepend: '/blog/category/' | prepend: site.baseurl}}">
              <i class="fas fa-tag fa-sm"></i> {{ category }}</a> &nbsp;
              {% endfor %}
          {% endif %}
    </p>
    </li>

    {% endfor %}
  </ul>

  {% include pagination.html %}

</div>

<br>

   



