---
title: "Downloads"
bg: grey
color: white
style: center
---

# **Downloads**
### *The "official" resources for Pokémon5E*

{% for member in site.data.books %}
<div class="banner_container">
<a href="{{ member.url }}" target="_blank">

<img src="{{ member.img }}">

<div class="banner_text">{{ member.title }}</div>

</a>
</div>	

{% endfor %}
