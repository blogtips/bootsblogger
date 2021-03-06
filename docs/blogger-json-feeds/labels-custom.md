---
layout: docs
title: Labels - custom
description: Menampilkan daftar label dari data JSON menggunakan beberapa komponen yang sesuai.
group: blogger-json-feeds
---

Menampilkan daftar label dari data JSON menggunakan beberapa komponen yang sesuai.

## Config

Nama fungsi: `labelsCustom`.

{% highlight html %}
<script>
var config = {
  postsPerPage: 10,
  badge: true|false,
  classes: {
    base: 'Base class',
    item: 'Item class',
    badge: 'badge badge-default badge-pill'
  }
}
</script>
{% endhighlight %}

**Catatan:** jika `badge: true`, dan Anda mempunyai banyak label, kecepatan memuat halaman mungkin akan berkurang.

## Examples

Menggunakan [Bootstrap list group](https://v4-alpha.getbootstrap.com/components/list-group/).

{% example html %}
<script>
var config = {
  postsPerPage: 10,
  badge: true,
  classes: {
    base: 'list-group',
    item: 'list-group-item list-group-item-action justify-content-between',
    badge: 'badge badge-default badge-pill'
  }
}
</script>
<script src="https://blogger.googleblog.com/feeds/posts/summary?max-results=0&amp;alt=json-in-script&amp;callback=labelsCustom"></script>
{% endexample %}

Menggunakan [Bootstrap dropdowns](https://v4-alpha.getbootstrap.com/components/dropdowns/).

{% example html %}
<div class="btn-group">
  <button class="btn btn-secondary dropdown-toggle" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Labels
  </button>
  <script>
  var config = {
    postsPerPage: 10,
    badge: true,
    classes: {
      base: 'dropdown-menu',
      item: 'dropdown-item',
      badge: 'badge badge-default badge-pill'
    }
  }
  </script>
  <script src="https://blogger.googleblog.com/feeds/posts/summary?max-results=0&amp;alt=json-in-script&amp;callback=labelsCustom"></script>
</div>
{% endexample %}

Menggunakan [Bootstrap navs](https://v4-alpha.getbootstrap.com/components/navs/).

{% example html %}
<script>
var config = {
  postsPerPage: 10,
  badge: true,
  classes: {
    base: 'nav flex-column',
    item: 'nav-link',
    badge: 'badge badge-default badge-pill'
  }
}
</script>
<script src="https://blogger.googleblog.com/feeds/posts/summary?max-results=0&amp;alt=json-in-script&amp;callback=labelsCustom"></script>
{% endexample %}
