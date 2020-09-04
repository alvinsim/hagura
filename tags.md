---
layout: post
title: What This MUSIC!
permalink: /tags/
content-type: eg
---

<style>
.category-content a {
    text-decoration: none;
    color: #4183c4;
}

.category-content a:hover {
    text-decoration: underline;
    color: #4183c4;
}
</style>

<h1>By Tags</h1>
<main>
    {% for tag in site.tags %}
      <h3 class="tag-headline" id="{{ tag | first }}">{{ tag | first }}</h3>
      {% for post in tag.last %}
        <li id="category-content" style="padding-bottom: 0.6em; list-style: none;">
		  <a href="{{post.url}}">{{ post.title }}</a>
	    </li>
      {% endfor %}
    {% endfor %}
    <br/>
    <br/>
</main>
