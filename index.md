Hello world

{{ site.description }}

   {% assign doclist = site.static_files  %}
   
       {% for doc in doclist %}
            {% if doc.name doc.name contains '.html' %}
- [{{ doc.name }}]({{ site.baseurl }}{{ doc.name }})
                
            {% endif %}
        {% endfor %}
   
