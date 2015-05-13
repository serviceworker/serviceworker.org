---
layout: default
featurettes:
  -
    icon: cogwheels
    title: The Service Worker
    body: A worker-like object that intercepts all network requests and lets you handle them in JavaScript.
  -
    icon: transfer
    title: The Fetch API
    body: XHR revamped.
  -
    icon: hdd
    title: The Cache API
    body: A simple cache for content retrieved from the Web (or generated), directly accessibly by the Service Worker.

ourresources:
  -
    icon: cogwheels
    title: Articles
    body: A worker-like object that intercepts all network requests and lets you handle them in JavaScript.
  -
    icon: transfer
    title: Presentations
    body: XHR revamped.
  -
    icon: hdd
    title: Slides
    body: A simple cache for content retrieved from the Web (or generated), directly accessibly by the Service Worker.
---

## What are service workers?

It's a new API to enable offline Web apps. (Like AppCache but that doesn't suck.)

Three parts:

{% include featurettes.html featurettes=page.featurettes col=3 %}

## Resources?

{% include featurettes.html featurettes=page.ourresources col=3 %}

## Show me code

<div class="row">
    <div class="col-md-6">
    <h3>/index.html</h3>
{% highlight html %}
{% include examples/index.html %}
{% endhighlight  %}
    </div>
    <div class="col-md-6">
    <h3>/service-worker.js</h3>
{% highlight javascript %}
{% include examples/service-worker.js %}
{% endhighlight  %}
    </div>
</div>

## An great intro by Jake Archibald

<iframe width="853" height="480" src="//www.youtube-nocookie.com/embed/4uQMl7mFB6g?rel=0" frameborder="0" allowfullscreen></iframe>

## When can I use it?

Current status of implementations can be found [here](https://jakearchibald.github.io/isserviceworkerready/).
