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
            <a href="{{ category.url }}" id="#{{ category | first | slugize }}">
                {{ category | first }}
            </a>
        </li>
    {% endfor %}
    </ul>
</aside>
