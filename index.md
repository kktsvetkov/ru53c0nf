---
# КТ: Слагайте последната година от архива, например за 2024 става `{% include_relative _archive/2024/index.md %}`
---

{% include_relative _archive/2024/index.md %}

{% for cat in site.categories %}
  <h3>{{ cat[0] }}</h3>
  <ul>
    {% for page in cat[1] %}
      <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
