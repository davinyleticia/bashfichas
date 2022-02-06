---
layout: post
title: '#{{ ficha }} {{ descen }}'
image: "{{ thumbnailen }}"
translated: "/projects/{{ ficha }}"
permalink: "/en/{{ ficha }}"
lang: "en"
pv:
  url: "/en/{{ previd }}"
  title: "{{ prevtitleen }}"
{% if next == "true" %}nt:
  url: "/en/{{ nextid }}"
  title: "{{ nexttitleen }}"
{% else %}nt:
  url: "https://gitfichas.com/en"
  title: "GitStudyCards | GitFichas"
{% endif %}---{% if subs == "true" %}
##### {{ subtitleen }}{% endif %}

<img alt="{{ alten }}" src="{{ highresen }}"><br><br>

| Command | Description |
|---------|-------------|{{ tableen }}
{: .styled-table}

{% if related == "true" %}<br>

Read more about this command in the following blog post:

<a href="{{ relatedsrcen }}">
  <strong>{{ relatedtexten }}</strong>
</a>
{% else %}<!--
<br>

Read more about this command in the following blog post:

<a href="{{ relatedsrcen }}">
  <strong>{{ relatedtexten }}</strong>
</a>
-->
{% endif %}