---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
title: UK BlueSCSI Page
---

{% assign cat_items = site.pages |  where_exp:"page", "page.tags contains 'uk'" %}
{% for page in cat_items %}

#### [{{page.cart_name}}]({{page.url}}) 

##### {{page.cart_description}} 

##### £{{page.cart_price}} 

#### [Add to cart](/cart#{{page.cart_itemid}}) 

{% endfor %}