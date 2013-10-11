---
title: Breadcrumbs in Jekyll
layout: code
category: code
---

Getting breadcrumbs back to a category page is pretty easy in Jekyll. If you have a way to create the category pages, that is (using a plugin).

## Breadcrumb code for post

{% highlight html %}
{% raw %}
<ol class="breadcrumb">
  <li><a href="/">Home</a></li>
  <li><a href="/categories/{{ page.categories.first }}">{{ page.categories.first }}</a></li>
  <li>{{ page.title }}</li>
</ol>
{% endraw %}
{% endhighlight %}

## Breadcrumb code for category

{% highlight html %}
{% raw %}
<ol class="breadcrumb">
  <li><a href="/">Home</a></li>
  <li>{{ page.title }}</li>
</ol>
{% endraw %}
{% endhighlight %}


