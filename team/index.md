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

{% include figure.html image="images/Vibha_Acharya.jpg" caption="Vibha Acharya, Postdoctoral" link="https://scholar.google.com/citations?user=TmiLyzcAAAAJ&hl=en" %}
{% include figure.html image="images/Asma_N_Cheema.jpg" caption="Asma N Cheema, Postdoctoral" link="https://scholar.google.com/citations?hl=en&user=5Tr99DEAAAAJ&view_op=list_works&sortby=pubdate" %}
{% include figure.html image="images/narges_zafari.jpg" caption="Narges Zafari, PhD" link="https://scholar.google.com/citations?user=949UI0QAAAAJ&hl=en"%}

{% endcapture %}

{% include grid.html style="square" content=content %}
