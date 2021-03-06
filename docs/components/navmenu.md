---
layout: docs
title: Navmenu
description: Navmenu adalah pembungkus untuk navigasi dan elemen lainnya.
group: components
---

Navmenu adalah pembungkus untuk navigasi dan elemen lainnya. Navmenu tampil secara vertikal, dengan dukungan *fixed left* dan *fixed right*, dan juga kemudahan untuk mengatur warna.

## Contents

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Basic example

Bungkus semua konten dengan `.navmenu`, dan tambahkan [skema warna](#color-schemes).

{% example html %}
<nav class="navmenu navmenu-light bg-faded">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
  <div class="navmenu-nav">
    <a class="nav-item nav-link active" href="#">Active</a>
    <a class="nav-item nav-link disabled" href="#">Disabled</a>
  </div>
</nav>
{% endexample %}

## Supported content

{% example html %}
<nav class="navmenu navmenu-light bg-faded">
  <!-- Brand -->
  <a class="navmenu-brand" href="#">Bootsblogger</a>

  <!-- Nav -->
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>

  <!-- Form -->
  <div class="navmenu-form">
    <form>
      <input class="form-control" type="text" placeholder="Search">
    </form>
  </div>

  <!-- Button -->
  <div class="navmenu-btn">
    <button type="button" class="btn btn-block btn-primary">Button</button>
  </div>

  <!-- Text -->
  <div class="navmenu-text">
    <p class="text-green">Bootsblogger is awesome.</p>
  </div>
</nav>
{% endexample %}

## Color schemes

Ubah warna navmenu dengan mengeset `background-color`, Anda dapat menggunakan [kelas utilitas warna]({{ site.baseurl }}/utilities/colors/#background-colors) atau menggunakan *custom styles*.

Gunakan `.navmenu-light` atau `.navmenu-inverse` untuk menyesuaikan warna teks dengan warna latar belakang yang terang atau gelap.

{% example html %}
<nav class="navmenu navmenu-light bg-faded">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}

{% example html %}
<nav class="navmenu navmenu-light" style="background-color: #e3f2fd;">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}

{% example html %}
<nav class="navmenu navmenu-inverse bg-blue">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}

{% example html %}
<nav class="navmenu navmenu-inverse" style="background-color: #ef6c00;">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}

## Dropdowns

{% example html %}
<nav class="navmenu navmenu-light bg-faded">
  <a class="navmenu-brand" href="#">Bootsblogger</a>
  <ul class="navmenu-nav">
    <li class="nav-item"><a class="nav-link" href="#">Nav item</a></li>
    <li class="nav-item"><a class="nav-link" href="#">Nav item again</a></li>
    <li class="nav-item dropdown">
      <a class="nav-link dropdown-toggle" href="javascript:;" id="navmenuDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        Dropdown link
      </a>
      <div class="dropdown-menu" aria-labelledby="navmenuDropdownMenuLink">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
      </div>
    </li>
    <li class="nav-item dropup">
      <a class="nav-link dropdown-toggle" href="javascript:;" id="navmenuDropupMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        Dropup
      </a>
      <div class="dropdown-menu" aria-labelledby="navmenuDropupMenuLink">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
      </div>
    </li>
  </ul>
</nav>
{% endexample %}

## Placement

{% example html %}
<nav class="navmenu navmenu-fixed-left navmenu-inverse bg-orange">
  <a class="navmenu-brand" href="#">Fixed left</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}

{% example html %}
<nav class="navmenu navmenu-fixed-right navmenu-inverse bg-orange">
  <a class="navmenu-brand" href="#">Fixed right</a>
  <div class="navmenu-nav">
    <a class="nav-item nav-link" href="#">Nav item</a>
    <a class="nav-item nav-link" href="#">Nav item again</a>
    <a class="nav-item nav-link" href="#">Another nav item</a>
  </div>
</nav>
{% endexample %}
