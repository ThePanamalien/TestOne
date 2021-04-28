# Testing Site - Carlos.P
___

<strong>Glossary</strong>

<nav>
<ul>
{% for pages in site.pages %}
<li><a href="{{ pages.url }}">{{ pages.title }}</a></li>
{% endfor %}
</ul>
</nav>


## Content to go below this point.
___

{% for pages in site.pages %}
  <p>{{ pages.content | markdownify }}</p>
{% endfor %}
