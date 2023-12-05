---
title: Lectures
illustration: avatar_glasses
---

# Ma liste de lecture

Quelques-unes de mes lectures (plus ou moins) récentes qui pourraient t'intéresser :

{% assign sorted = site.readings | sort: 'read' | reverse  %}
{% for reading in sorted %}
* {{ reading.title }}*, de {{ reading.author }}*
{% endfor %}