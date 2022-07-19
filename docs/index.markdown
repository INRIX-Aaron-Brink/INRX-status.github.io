---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
<ul>
{% for service in site.data.all-services %}
  <li>
    <a href="{{ service.name }}.html">
      {{ service.name }}
      
    </a>
    {{ service.productionUrl}}
    {% for dep in service.dependencies %}
      <li>{{dep}}</li>
    {% endfor %}
  </li>
{% endfor %}
</ul>
<p>hello</p>
