---
title: Video - Entertainment
---

## 电影

{% if site.data.entertainment.video.movie %}
{% assign video_movie = site.data.entertainment.video.movie %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for video in video_movie %}
    {% if video.title != "" %}
    <div class="col">
      {% if video.movie_douban_slug and video.movie_douban_slug != '' %}
        <a class="card" target="_blank" href="https://movie.douban.com/subject/{{video.movie_douban_slug}}/">
          {% if video.movie_douban_ico and video.movie_douban_ico != '' %}
          <img class="card-img-top lazyload" data-src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/{{video.movie_douban_ico}}.webp" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{video.url}}">
          {% if video.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{video.storageIco}}" alt=""/>
          {% else if video.ico %}
            <img class="card-img-top lazyload" data-src="{{video.ico}}" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## 电视剧

{% if site.data.entertainment.video.teleplay %}
{% assign video_teleplay = site.data.entertainment.video.teleplay %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for video in video_teleplay %}
    {% if video.title != "" %}
    <div class="col">
      {% if video.movie_douban_slug and video.movie_douban_slug != '' %}
        <a class="card" target="_blank" href="https://movie.douban.com/subject/{{video.movie_douban_slug}}/">
          {% if video.movie_douban_ico and video.movie_douban_ico != '' %}
          <img class="card-img-top lazyload" data-src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/{{video.movie_douban_ico}}.webp" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{video.url}}">
          {% if video.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{video.storageIco}}" alt=""/>
          {% else if video.ico %}
            <img class="card-img-top lazyload" data-src="{{video.ico}}" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## 动漫

{% if site.data.entertainment.video.anime %}
{% assign video_anime = site.data.entertainment.video.anime %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for video in video_anime %}
    {% if video.title != "" %}
    <div class="col">
      {% if video.movie_douban_slug and video.movie_douban_slug != '' %}
        <a class="card" target="_blank" href="https://movie.douban.com/subject/{{video.movie_douban_slug}}/">
          {% if video.movie_douban_ico and video.movie_douban_ico != '' %}
          <img class="card-img-top lazyload" data-src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/{{video.movie_douban_ico}}.webp" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{video.url}}">
          {% if video.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{video.storageIco}}" alt=""/>
          {% else if video.ico %}
            <img class="card-img-top lazyload" data-src="{{video.ico}}" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% endif %}
    </div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}

## 特摄片

{% if site.data.entertainment.video.tokusatsu %}
{% assign video_tokusatsu = site.data.entertainment.video.tokusatsu %}
<div class="row row-cols-2 row-cols-sm-4 row-cols-md-6">
  {% for video in video_tokusatsu %}
    {% if video.title != "" %}
    <div class="col">
      {% if video.movie_douban_slug and video.movie_douban_slug != '' %}
        <a class="card" target="_blank" href="https://movie.douban.com/subject/{{video.movie_douban_slug}}/">
          {% if video.movie_douban_ico and video.movie_douban_ico != '' %}
          <img class="card-img-top lazyload" data-src="https://img3.doubanio.com/view/photo/s_ratio_poster/public/{{video.movie_douban_ico}}.webp" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
          </div>
        </a>
      {% else %}
        <a class="card" target="_blank" href="{{video.url}}">
          {% if video.storageIco %}
            <img class="card-img-top lazyload" data-src="{{site.storageUrl.favicon}}/{{video.storageIco}}" alt=""/>
          {% else if video.ico %}
            <img class="card-img-top lazyload" data-src="{{video.ico}}" alt=""/>
          {% endif %}
          <div class="card-body p-2">
            <h5 class="card-title text-truncate my-2">{{ video.titleCn }} {{ video.title }}</h5>
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

{% if site.data.entertainment.video.websites.original %}
{% assign video_original_websites = site.data.entertainment.video.websites.original %}
<ul>
  {% for website in video_original_websites %}
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

{% if site.data.entertainment.video.websites.other %}
{% assign video_other_websites = site.data.entertainment.video.websites.other %}
<ul>
  {% for website in video_other_websites %}
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
