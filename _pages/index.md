---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
permalink: /
# layout: home
layout: default
title: Home
permalink: /
---

# Hi

Check out these other pages:

{% include tooltip.html position="top" text="This is a tooltip!" %}

{% for item in site.data.skills %}
<h4>{{ item.category }}</h4>
<ul>
    {% for skill in item.skills %}
    <li class="skill">{{ skill.name }} - {{ skill.rating }}</li>
    {% endfor %}
</ul>
{% endfor %}


