---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---


<div class="home">
  <div id="catherine">
      <div id="root"></div>
  </div>

<button>{% for my_page in site.pages %}
          {% if my_page.title %}
          <a class="rules" href="{{ my_page.url | prepend: site.baseurl }}">VIEW THE RULES</a>
          {% endif %}
        {% endfor %}</button>

  <h1 class="page-heading"></h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

</div>