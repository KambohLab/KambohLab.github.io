---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Dr. M. Ilyas Kamboh leads the laboratory, with Annie Bedison serving as the lab manager. For inquiries, including potential collaborations or requests for summary statistics, please feel free to contact us using the information provided below. We welcome the opportunity to discuss future partnerships and data sharing.

{%
  include button.html
  type="email"
  text="hugen-kambohlab@pitt.edu"
  link="hugen-kambohlab@pitt.edu"
%}
{%
  include button.html
  type="phone"
  text="(412) 624-3021"
  link="+1-412-624-3021"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://maps.app.goo.gl/LzATGq8RpWrznHqX7"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/Prof_Ilyas_Kamboh.jpg"
  caption="Dr. M. Ilyas Kamboh"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Annie Bedison, MS"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}

{% endcapture %}

{% capture col2 %}


{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}
