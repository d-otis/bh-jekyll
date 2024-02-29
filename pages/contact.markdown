---
title: Contact
permalink: /contact
---

{% assign email_address = '' %}
{% for letter in site.data.address.letters %}
{% assign email_address = email_address | prepend: letter %}
{% endfor %}

<a href="mailto:{{ email_address | encode_email }}"><i class="fas fa-envelope"></i> Email Us</a>

{% for env in site.env %}
{{ env }}
{% endfor %}
