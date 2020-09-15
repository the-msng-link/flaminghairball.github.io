---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# layout: home
---
👋🏼Welcome

I work on [Houseparty](https://apps.apple.com/us/app/houseparty/id1065781769) at [Epic Games](https://epicgames.com/)

I made [Rusty's Dump Truck Service](https://apps.apple.com/us/app/rustys-dump-truck-service/id1513836293) 🚚

🏍 Travel

I ride motorcycles whenever the sun is out (or when it's not)

👓Workbench

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>