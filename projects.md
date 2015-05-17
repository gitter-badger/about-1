---
layout: page
title: Projects
permalink: /projects/
---

{% for project in site.data.projects %}
<div class="media">
    <a href="#" class="pull-left">
        <img height="40px" width="40px" src="/assets/img/{{ project.logo }}" class="media-object" alt="{{ project.name }} logo">
    </a>
    <div class="media-body">
        <h4 class="media-heading">
            <b>{{ project.name }}</b>
        </h4>
        <p>{{ project.summary }}</p>
        <p>
            <a class="btn btn-default btn-xs" target="_blank" href="{{ project.web }}">Web</a>
            {% if project.repo != '' %}
                <a class="btn btn-default btn-xs" href="{{ project.repo }}" target="_blank">Contribute</a>
            {% endif %}
        </p>
    </div>
</div>
{% endfor %}