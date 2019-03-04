---
layout: page
title: Publication
permalink: /publication/
---
{% assign journal_count = 0 %}
<!-- <h1>Preprint</h1> -->
<div >
<ol class="number-listing">
{% for post in site.categories.publication %}
    {% if post.type contains "preprint" %}
        {% assign journal_count = journal_count | plus: 1 %}
        <li>
        "{{ post.title }}"
        <br>{{ post.authors | replace_first: 'Mirza M. Elahi', '<b>Mirza M. Elahi</b>'}}
        <br>
            <a href="{{ post.fulltext }}">
            <b><i>{{ post.journal }}</i></b>,
            {% if post.volume %}
            vol. {{ post.volume }}
            {% endif %}
            {% if post.issue %}
            :{{ post.issue }},
            {% endif %}
            {% if post.pages %}
            pp. {{ post.pages }},
            {% endif %}
            {{ post.year }}</a>.
            </br>

        </li>
    {% endif %}
{% endfor %}
</ol>
</div>


<h1>Journal</h1>
<div >
<ol class="number-listing">
{% for post in site.categories.publication %}
    {% if post.type contains "journal" %}
        {% assign journal_count = journal_count | plus: 1 %}
        <li>
        "{{ post.title }}"
        <br>{{ post.authors | replace_first: 'Mirza M. Elahi', '<b>Mirza M. Elahi</b>'}}
        <br>
            <a href="{{ post.fulltext }}"><b><i>{{post.journal}}</i></b>{% if post.volume %}, vol. {{ post.volume }}{% endif %}{% if post.issue %}, no. {{ post.issue }}{% endif %}{% if post.pages %}, pp. {{ post.pages }}{% endif %}, {{ post.year }}</a>.
            </br>
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
                    "{{ post.title }}"
                    <br>{{ post.authors | replace_first: 'Mirza M. Elahi', '<b>Mirza M. Elahi</b>'}}
                    <br>
                        <a href="{{ post.fulltext }}"><i>{{post.journal}}</i>{% if post.volume %}, vol. {{ post.volume }}{% endif %}{% if post.issue %}, no. {{ post.issue }}{% endif %}{% if post.pages %}, pp. {{ post.pages }}{% endif %}, {{ post.year }}</a>.
                    </br>
                </li>
            {% endif %}
        {% endfor %}
    </ol>
</div>

<h1>Graphical Presentation </h1>
<div>
<img class="Picture" src="{{ site.baseurl }}/images/scholarPlot.png" alt="timeline" width="1000" style="padding: 10px 0 0 0;">
</div>
