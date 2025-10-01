---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team Members

Our multidisciplinary team includes talented scientists with expertise in neuroscience, epidemiology, genetics and genomics, biostatistics, and bioinformatics.

They collaborate to investigate the genetic architecture of complex diseases, particularly Alzheimer’s disease and related dementias. Over the past 20+ years, our lab has trained and mentored more than 10 postdoctoral fellows, 30 PhD students, and 50 master’s students, all of whom have made valuable contributions to the field.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'professor'" %}
{% include list.html data="members" component="portrait" filter="role != 'professor'" %}

{% include section.html background="images/AI_banner2.png" dark=true %}

{% include section.html %}

## Postdoctoral Fellows & PhD Students

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
