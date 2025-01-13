---
title: "Novel - Entertainment"
---

## 连载

{% if site.data.entertainment.novel.serial %}
{% assign novel_serial = site.data.entertainment.novel.serial %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for novel in novel_serial %}
    {% if novel.title != "" %}
    <div class="col">
      {% if novel.qidian_slug and novel.qidian_slug != '' %}
        <a class="card" target="_blank" href="https://www.qidian.com/book/{{novel.qidian_slug}}/">
          <img class="card-img-top lazyload" data-src="https://bookcover.yuewen.com/qdbimg/349573/{{novel.qidian_slug}}/150.webp" alt=""/>
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{novel.url}}">
          {% if novel.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{novel.storageIco}}" alt=""/>
          {% else if novel.ico %}
            <img class="card-img-top lazyload" data-src="{{novel.ico}}" alt=""/>
          {% endif %}
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## 完结

{% if site.data.entertainment.novel.finished %}
{% assign novel_finished = site.data.entertainment.novel.finished %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for novel in novel_finished %}
    {% if novel.title != "" %}
    <div class="col">
      {% if novel.qidian_slug and novel.qidian_slug != '' %}
        <a class="card" target="_blank" href="https://www.qidian.com/book/{{novel.qidian_slug}}/">
          <img class="card-img-top lazyload" data-src="https://bookcover.yuewen.com/qdbimg/349573/{{novel.qidian_slug}}/150.webp" alt=""/>
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{novel.url}}">
          {% if novel.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{novel.storageIco}}" alt=""/>
          {% else if novel.ico %}
            <img class="card-img-top lazyload" data-src="{{novel.ico}}" alt=""/>
          {% endif %}
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## 断更

{% if site.data.entertainment.novel.suspend %}
{% assign novel_suspend = site.data.entertainment.novel.suspend %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for novel in novel_suspend %}
    {% if novel.title != "" %}
    <div class="col">
      {% if novel.qidian_slug and novel.qidian_slug != '' %}
        <a class="card" target="_blank" href="https://www.qidian.com/book/{{novel.qidian_slug}}/">
          <img class="card-img-top lazyload" data-src="https://bookcover.yuewen.com/qdbimg/349573/{{novel.qidian_slug}}/150.webp" alt=""/>
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{novel.url}}">
          {% if novel.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{novel.storageIco}}" alt=""/>
          {% else if novel.ico %}
            <img class="card-img-top lazyload" data-src="{{novel.ico}}" alt=""/>
          {% endif %}
          <div class="card-body px-2 py-0">
            <h5 class="card-title text-truncate my-1">{{ novel.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## websites

**正版**

{% if site.data.entertainment.novel.websites.original %}
{% assign novel_original_websites = site.data.entertainment.novel.websites.original %}
<ul>
  {% for website in novel_original_websites %}
    {% if website.title != "" %}
    <li>
      <a target="_blank" href="{{website.url}}">
        {% if website.storageIco %}
          <img class="lazyload" data-src="{{site.storageUrl.favicon}}/{{website.storageIco}}" alt=""/>
        {% else if website.ico %}
          <img class="lazyload" data-src="{{website.ico}}" alt=""/>
        {% endif %}
        {{ website.title }}
      </a>
    </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

**其它**

{% if site.data.entertainment.novel.websites.other %}
{% assign novel_other_websites = site.data.entertainment.novel.websites.other %}
<ul>
  {% for website in novel_other_websites %}
    {% if website.title != "" %}
    <li>
      <a target="_blank" href="{{website.url}}">
        {% if website.storageIco %}
          <img class="lazyload" data-src="{{site.storageUrl.favicon}}/{{website.storageIco}}" alt=""/>
        {% else if website.ico %}
          <img class="lazyload" data-src="{{website.ico}}" alt=""/>
        {% endif %}
        {{ website.title }}
      </a>
    </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}
