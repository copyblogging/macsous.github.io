---
layout: page
title: Livros
permalink: /livros/
---
{% for livros in site.categories %}
    <article class="art">
        <header>
          <h1><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h1>
          <p id="info1">Por {{ post.author }} em {{ post.date | date: "%-d/%m/%Y" }} &#8211; <span>{{ post.categories }}</span>.</p>
        </header>
        <div>{{ post.summary }}</div>
        <p id="sm"><a href="{{ post.url | prepend: site.baseurl }}">Saiba mais!</a></p>
    </article>
    <div id="lin"></div>
{% endfor %}
