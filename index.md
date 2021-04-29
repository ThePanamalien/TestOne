# Testing Site - Carlos.P
___

<style>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #4181f9;
}

li {
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  background-color: #ffe400;
}
</style>

<strong>Glossary</strong>

<nav>
<ul>
{% for pages in site.pages %}
<li>
  <a href="{{ pages.url | prepend: site.baseurl }}">
   <h4>{{ pages.title }}</h4>
  </a>
  </li>
{% endfor %}
</ul>
</nav>


## Content to go below this point.
___

{% for pages in site.pages %}
  <p>{{ pages.content | markdownify }}</p>
{% endfor %}
