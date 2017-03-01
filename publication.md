---
layout: page
title: Publication
permalink: /publication/
---
{% assign journal_count = 0 %}
<h1>Journal</h1>
<div >
<ol class="number-listing">
{% for post in site.categories.publication %}
    {% if post.type contains "journal" %}
        {% assign journal_count = journal_count | plus: 1 %}
        <li>
        <a href="{{ post.fulltext }}">{{ post.title }}</a>
        <br>{{ post.authors | replace_first: 'Mirza M. Elahi', '<b>Mirza M. Elahi</b>'}}, <i>{{ post.journal }}</i>,
        {% if post.volume %}
        vol. {{ post.volume }}
        {% endif %}
        {% if post.issue %}
        :{{ post.issue }}
        {% endif %}
        ,
        {% if post.pages %}
        pp. {{ post.pages }},
        {% endif %}
        {{ post.year }}

        </li>
    {% endif %}
{% endfor %}
</ol>
</div>
<h1>Conference Proceedings</h1>

<div>
<ol class="number-listing">
{% for post in site.categories.publication %}
{% if post.type contains "conference" %}
{% assign journal_count = journal_count | plus: 1 %}
<li>
<a href="{{ post.fulltext }}">{{ post.title }}</a>
<br>{{ post.authors | replace_first: 'Mirza M. Elahi', '<b>Mirza M. Elahi</b>'}}, <i>{{ post.journal }}</i>,
{% if post.volume %}
vol. {{ post.volume }}
{% endif %}
{% if post.issue %}
:{{ post.issue }}
{% endif %}
,
{% if post.pages %}
pp. {{ post.pages }},
{% endif %}
{{ post.year }}
</li>
{% endif %}
{% endfor %}
</ol>
</div>
