---
layout: default
---

# # cat about.txt
{:id="about"}

Just a blog about some stuff.

# # cat contact.txt
{:id="contact"}

I don't know why you would want to but you can contact me: [email](mailto:root@deleteroot.com).

# # cat posts.txt
{:id="posts"}

<ul>
{% for post in site.categories.posts %}

{% if post.en %}
<li>{{ post.title }} :: <a href="{{ post.url }}" title="{{ post.description }}">link</a></li>
{% endif %}

{% endfor %}
</ul>
