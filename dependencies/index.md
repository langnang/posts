---
title: Dependencies

baseNpmUrl: https://www.npmjs.com/package

cdns:
  - name: github
    homepage: https://github.com/
    storageIco: /github.ico

npm_cdns:
  - name: npmjs
    homepage: https://npmjs.com/
    storageIco: /npmjs.ico
    packageUrl: https://npmjs.com/
  - name: cdnjs
    homepage: https://cdnjs.com/
    storageIco: /cdnjs.ico
    packageUrl: https://cdnjs.com/
  - name: jsdelivr
    homepage: https://jsdelivr.com/
    storageIco: /jsdelivr.ico
    packageUrl: https://jsdelivr.com/
  - name: unpkg 
    homepage: https://unpkg.com/
    storageIco: /unpkg.ico
    packageUrl: https://unpkg.com/
---

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.cdns %}
    <a class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
    <a class="d-inline-flex" href="https://github.com/"><img src="{{site.storageUrl.favicon}}/github.ico"/></a>
</div>

## NPM

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.npm_cdns %}
    <a class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

<!-- UNPKG -->
<!-- <link rel="stylesheet" href="" /> -->
<!-- <script src=""></script> -->

```html
<!-- UNPKG -->
<!--  -->
<link rel="stylesheet" href="https://www.unpkg.com/{package}" />
<script src="https://www.unpkg.com/{package}"></script>
<!-- OR -->
<!-- https://www.unpkg.com/{package}@{version} -->
<link rel="stylesheet" href="https://www.unpkg.com/{package}@{version}" />
<script src="https://www.unpkg.com/{package}@{version}"></script>
<!-- OR -->
<!-- https://www.unpkg.com/{package}@{version}/{file} -->
<script src="https://www.unpkg.com/{package}@{version}"></script>

<!-- NPM -->

<!-- jsDelivr -->

```

{% if site.data.dependencies.npm_packages %}
<ul>
  {% for package in site.data.dependencies.npm_packages %}
    <li>
      {% if package.github and package.github.user and package.github.repo %}
        <a href="https://github.com/{{package.github.user}}/{{package.github.repo}}">
          <img src="{{site.storageUrl.favicon}}/github.ico" alt="">
        </a>
      {% endif %}
      {% for cdn in page.npm_cdns %}
        <a href="{{cdn.packageUrl}}/{{package.name}}">
          {% if cdn.storageIco %}
            <img src="{{site.storageUrl.favicon}}{{cdn.storageIco}}" alt=""/>
          {% else if cdn.ico %}
            <img src="{{cdn.ico}}" alt=""/>
          {% endif %}
        </a>
      {% endfor %}
      {% if package.storageIco or package.ico and package.homepage %}
        <a href="{{package.homepage}}">
          {% if package.storageIco %}
            <img src="{{site.storageUrl.favicon}}{{package.storageIco}}" alt=""/>
          {% else if package.ico %}
            <img src="{{package.ico}}" alt=""/>
          {% endif %}
        </a>
      {% endif %}
      <code class="language-plaintext highlighter-rouge">{{package.name}}</code>:
      {% if package.description %}
        <span>{{package.description}}</span>
      {% endif %}
    </li>
  {% endfor %}
</ul>
{% endif %}

## Composer

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
    <a class="d-inline-flex" href="https://packagist.org/"><img src="{{site.storageUrl.favicon}}/packagist.ico"/></a>
</div>

```bash
composer require {package}
```

- `laravel/laravel`
- `laravel/lumen`
- `phpspider`

## RubyGems

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
    <a class="d-inline-flex" href="https://rubygems.org/"><img src="{{site.storageUrl.favicon}}/rubygems.ico"/></a>
</div>

**Gemfile**

```ruby
gem '{package}', '~>{version}'
```

**install**

```bash
gem install {package}
```

- jekyll  3.9.5
- github-pages-health-check  1.18.2
- github-pages  231
- html-pipeline  2.14.3
- jekyll-avatar  0.8.0
- jekyll-coffeescript  1.2.2
- jekyll-commonmark-ghpages  0.4.0
- jekyll-default-layout  0.1.5
- jekyll-feed  0.17.0
- jekyll-gist  1.5.0
- jekyll-github-metadata  2.16.1
- jekyll-include-cache  0.2.1
- jekyll-mentions  1.6.0
- jekyll-optional-front-matter  0.3.2
- jekyll-paginate  1.1.0
- jekyll-readme-index  0.3.0
- jekyll-redirect-from  0.16.0
- jekyll-relative-links  0.6.1
- jekyll-remote-theme  0.4.3
- jekyll-sass-converter  1.5.2
- jekyll-seo-tag  2.8.0
- jekyll-sitemap  1.4.0
- jekyll-swiss  1.0.0
- jekyll-theme-architect  0.2.0
- jekyll-theme-cayman  0.2.0
- jekyll-theme-dinky  0.2.0
- jekyll-theme-hacker  0.2.0
- jekyll-theme-leap-day  0.2.0
- jekyll-theme-merlot  0.2.0
- jekyll-theme-midnight  0.2.0
- jekyll-theme-minimal  0.2.0
- jekyll-theme-modernist  0.2.0
- jekyll-theme-primer  0.6.0
- jekyll-theme-slate  0.2.0
- jekyll-theme-tactile  0.2.0
- jekyll-theme-time-machine  0.2.0
- jekyll-titles-from-headings  0.5.3
- jemoji  0.13.0
- kramdown-parser-gfm  1.1.0
- kramdown  2.4.0
- liquid  4.0.4
- minima  2.5.1
- nokogiri  1.15.5
- rouge  3.30.0
- ruby  2.7.4
- safe_yaml  1.0.5
- sass  3.7.4
- jekyll-get-json: Import remote JSON data into the data for a Jekyll site

## Pipy

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
    <a class="d-inline-flex" href="https://pypi.org/"><img src="{{site.storageUrl.favicon}}/pypi.ico"/></a>
</div>
