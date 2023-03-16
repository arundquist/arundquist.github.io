Hello world

{{ site.description }}

   {% assign doclist = site.static_files  %}
    <ul>
       {% for doc in doclist %}
            {% if doc.name contains '.md' or doc.name contains '.html' %}
                <li><a href="{{ site.baseurl }}{{ doc.name }}">{{ doc.name }}</a></li>
            {% endif %}
        {% endfor %}
    </ul>
