---
layout: page
title: Publications and Talks
permalink: /pubandtalks/
---

#Talks
{% for publication in site.data.publications %}
  <div class="media">
      <div class="media-body">
          <h4 class="media-heading"><a target="=_blank" href="{{ publication.url }}">{{ publication.title }}</a></h4>
          <p>
              <i>{{ publication.authors }}</i>
              <br>
              <i><b>{{ publication.location }}</b></i>
              <br>
          </p>
          <p>{{ publication.summary }}</p>
      </div>
  </div>
{% endfor %}




