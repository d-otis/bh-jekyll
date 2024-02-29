---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---

{% include header.markdown %}

<div class="container">
  <div class="row">
    <div class="page col-sm-12 col-md-8 offset-md-2">
    {% unless page.name contains 'index' %}
      <h3 class="text-right mb-4">[{{ page.title | downcase }}]</h3>
    {% endunless %}
      {{ content }}
    </div>
    <!-- end of .page .col-sm-8 etc -->
  </div>
  <!-- end of .row -->
</div>

{% include footer.html %}
