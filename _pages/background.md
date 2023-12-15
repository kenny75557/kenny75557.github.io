---
layout: archive
author_profile: true
permalink: /background/
---

<!-- {% include base_path %} -->
# Education
* M.S. in Computer Science, National Chung-Hsing University, 2022

* B.S. in Computer Science and Information Engineering, Fu Jen Catholic University, 2020

# Work Experience
<p></p>
{% for post in site.data.experience.main  %}
<div style="display: flex; justify-content: space-between; margin-left: 50px; text-indent: -30px;">
{% if post.link %}
    <a href="{{ post.link }}">
        <b>{{ post.place }}</b>
    </a>
{% else %}
    <b>{{ post.place }}</b>
{% endif %}
{{post.time}}
</div>
<p style="margin-left: 50px">
{{post.title}} 
</p>
{% endfor %}

