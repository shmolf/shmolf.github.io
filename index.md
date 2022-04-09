<div class="flex">
    <main>
        Main Content here, please
        <h1>🚧Blog Under Construction🚧</h1>
    </main>
    <aside>
        <ul>
        {% for post in site.posts | slice: 0, 5 %}
            <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
            </li>
        {% endfor %}
        </ul>
    </aside>
</div>
