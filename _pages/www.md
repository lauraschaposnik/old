---
layout: blog
permalink: /www/
title: What Will We
nav: false
youtube: https://www.youtube.com/embed/EtMYl0Q15C0
heading: What Will We
---


<br>
   
<h2> What Will We </h2>
     
    
<br>

What Will We… do the same? Or perhaps change? 

 
Since early 2020 scientists across the world begun changing the way they approach research activities: these changes have continued to fluctuate and are now slowly converging into what we will likely call our <i>new normal</i>, a quasi stable point in which we find ourselves comfortable having rediscovered our boundaries and strengths.  

In this series of interviews with mathematicians (and scientists) from around the world, we look at what habits they have developed in the last years which they will nurture in the future, and which activities they think will no longer deserve their time or attention. We will learn from each other with hopes of making our academic life each day more enjoyable and stimulating, and at the same time give a glimpse of why each of us wakes up every morning wanting do do science. 
  
Researchers have studied <i>  job  satisfaction  of academics in times of transformation </i> from different perspectives -- some decades ago, for instance, academics in South Africa  from departments at a residential and a distance education institution were asked to answer a survey with hopes of identifying factors causing satisfaction and dissatisfaction  and, among other findings, significant correlations between job satisfaction and physical conditions and support  were determined <b> <a href="https://doi.org/10.10520/EJC37233">[2006]</a></b>. In the current times of transformation, among mathematicians we notice a similar perception of sources of satisfaction within an academic job. 
  
 <blockquote> 
Over the years we learn to appreciate collaborations, interactions between areas of mathematics and the physicality of our jobs. 
</blockquote>
 
 Already some decades ago researchers were considering different factors that could influence the success of online (or distance) learning <a href="https://doi.org/10.1108/09513540010344731"><b>[2000]</b></a>, and the last couple of years might have been the transformation period needed for online education to be popularized and finally <i> be here to stay</i>. 

 <blockquote> 
Online education is here to stay, and we are quickly learning how to make the most of it both for research and for education. 
</blockquote>

That said, whilst the peak interest in an <i> online degree </i> was reached in August 2020 during the COVID-19 pandemic, it would seem the interest is reaching a <a href="https://trends.google.com">5-year low in 2022</a> and thus the "online education" that is here to stay should be thought as some kind of well balanced hybrid academic setting which makes the most of both the online and in person worlds. 


<br>

 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/onlinedegree.png" title="Online degree interest" class="img-fluid rounded z-depth-1" %}
    </div>
     </div>

 <br>
 <br>

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

 
<h3> <a id="conclusions_resources"> Resources and acknowledgements</a></h3>
   
There are a number of resources that have inspired or been used in this notebook, some of which are cited along the way. They are also collected here for reference purposes:

- <b>[2000] </b> Volery, T. and Lord, D. (2000), "Critical success factors in online education", International Journal of Educational Management, Vol. 14 No. 5, <a href="https://doi.org/10.1108/09513540010344731">https://doi.org/10.1108/09513540010344731</a>


- <b>[2006] </b> S. Schulze, "Factors influencing the job satisfaction of academics in higher education", <i>Higher Education South Africa (HESA)</i>, 2006 <a href="https://doi.org/10.10520/EJC37233">https://doi.org/10.10520/EJC37233</a>. 


