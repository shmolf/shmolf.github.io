<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
<aside>
    <ul>
    {% for category in site.categories %}
        <li>
            <a href="{{ categories.url }}" id="#{{ category | slugize }}">
                {{ categories.title }}
            </a>
        </li>
    {% endfor %}
    </ul>
</aside>
