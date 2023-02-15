---
layout: default
title: Liste de lecture
illustration: avatar_glasses
---

# Liste de lecture

Quelques-unes de mes lectures récentes qui pourraient t'intéresser :

{% assign sorted = site.readings | sort: 'read' | reverse  %}
{% for reading in sorted %}
* {{ reading.title }}, de *{{ reading.author }}*
{% endfor %}