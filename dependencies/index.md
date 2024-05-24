---
title: Dependencies

baseNpmUrl: https://www.npmjs.com/package

cdns:
  - name: github
    homepage: https://github.com/
    storageIco: github.ico
    ico: 
  - name: gitlab
    homepage: https://gitlab.com/
    storageIco: gitlab.ico
  - name: gitee
    homepage: https://gitee.com/
    storageIco: gitee.ico
  - name: bitbucket
    homepage: https://bitbucket.org/
    storageIco: bitbucket.ico
  - name: sourceforge  
    homepage: https://sourceforge.net/  
    storageIco: sourceforge.ico
  - name: coding
    homepage: https://coding.net/
    storageIco: coding.ico

npm_cdns:
  - name: npmjs
    homepage: https://npmjs.com/
    storageIco: npmjs.ico
    packageUrl: https://npmjs.com/
  - name: cdnjs
    homepage: https://cdnjs.com/
    storageIco: cdnjs.ico
    packageUrl: https://cdnjs.com/
  - name: jsdelivr
    homepage: https://jsdelivr.com/
    storageIco: jsdelivr.ico
    packageUrl: https://jsdelivr.com/
  - name: unpkg 
    homepage: https://unpkg.com/
    storageIco: unpkg.ico
    packageUrl: https://unpkg.com/
  - name: bootcdn 
    homepage: https://bootcdn.cn/
    storageIco: bootcdn.ico
    packageUrl: https://bootcdn.cn/  

composer_cdns:
  - name: packagist
    homepage: https://packagist.org/
    storageIco: packagist.ico
    packageUrl: https://packagist.org/packages

ruby_cnds:
  - name: rubygems
    homepage: https://rubygems.org/
    storageIco: rubygems.ico
    packageUrl: https://rubygems.org/gems/

pypi_cdns:
  - name: pypi
    homepage: https://pypi.org/
    storageIco: pypi.ico
    packageUrl: https://pypi.org/project/
---

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.cdns %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

## NPM

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.npm_cdns %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
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
{% assign npm_packages = site.data.dependencies.npm_packages %}
<ul>
  {% for package in npm_packages %}
    {% if package.name %}
      <li>
        {% for cdn in page.npm_cdns %}
          <a target="_blank" href="{{cdn.packageUrl}}/{{package.name}}">
            {% if cdn.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}" alt=""/>
            {% else if cdn.ico %}
              <img src="{{cdn.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endfor %}
        {% if package.github_user and package.github_repo %}
          <a target="_blank" href="https://github.com/{{package.github_user}}/{{package.github_repo}}">
            <img src="{{site.storageUrl.favicon}}/github.ico" alt="">
          </a>
        {% endif %}
        {% if package.storageIco or package.ico and package.homepage %}
          <a target="_blank" href="{{package.homepage}}">
            {% if package.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{package.storageIco}}" alt=""/>
            {% else if package.ico %}
              <img src="{{package.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endif %}
        <img src="https://img.shields.io/npm/dt/{{package.name}}" />
        <code class="language-plaintext highlighter-rouge">{{package.name}}</code>:
        {% if package.description %}
          <span>{{package.description}}</span>
        {% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

## Composer

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.composer_cdns %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

**intall**

```bash
composer require {package}

# 更新 autoload
composer dump-autoload
```

{% if site.data.dependencies.composer_packages %}
{% assign composer_packages = site.data.dependencies.composer_packages %}
<ul>
  {% for package in composer_packages %}
    {% if package.name %}
      <li>
        {% for cdn in page.composer_cdns %}
          <a target="_blank" href="{{cdn.packageUrl}}/{{package.name}}">
            {% if cdn.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}" alt=""/>
            {% else if cdn.ico %}
              <img src="{{cdn.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endfor %}
        {% if package.github_user and package.github_repo %}
          <a target="_blank" href="https://github.com/{{package.github_user}}/{{package.github_repo}}">
            <img src="{{site.storageUrl.favicon}}/github.ico" alt="">
          </a>
        {% endif %}
        {% if package.storageIco or package.ico and package.homepage %}
          <a target="_blank" href="{{package.homepage}}">
            {% if package.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{package.storageIco}}" alt=""/>
            {% else if package.ico %}
              <img src="{{package.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endif %}
        <img src="https://img.shields.io/packagist/dt/{{package.name}}" />
        <code class="language-plaintext highlighter-rouge">{{package.name}}</code>:
        {% if package.description %}
          <span>{{package.description}}</span>
        {% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

## Ruby

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.ruby_cnds %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

**Gemfile**

```ruby
gem '{package}', '~>{version}'
```

**install**

```bash
gem install {package}
```

{% if site.data.dependencies.ruby_packages %}
{% assign ruby_packages = site.data.dependencies.ruby_packages %}
<ul>
  {% for package in ruby_packages %}
    {% if package.name %}
      <li>
        {% for cdn in page.ruby_cnds %}
          <a target="_blank" href="{{cdn.packageUrl}}/{{package.name}}">
            {% if cdn.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}" alt=""/>
            {% else if cdn.ico %}
              <img src="{{cdn.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endfor %}
        {% if package.github_user and package.github_repo %}
          <a target="_blank" href="https://github.com/{{package.github_user}}/{{package.github_repo}}">
            <img src="{{site.storageUrl.favicon}}/github.ico" alt="">
          </a>
        {% endif %}
        {% if package.storageIco or package.ico and package.homepage %}
          <a target="_blank" href="{{package.homepage}}">
            {% if package.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{package.storageIco}}" alt=""/>
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
    {% endif %}
  {% endfor %}
</ul>
{% endif %}

## PyPI

<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.pypi_cdns %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

**intall**

```bash
pip install {package}
```

{% if site.data.dependencies.pypi_packages %}
{% assign pypi_packages = site.data.dependencies.pypi_packages %}
<ul>
  {% for package in pypi_packages %}
    {% if package.name %}
      <li>
        {% for cdn in page.pypi_cdns %}
          <a target="_blank" href="{{cdn.packageUrl}}/{{package.name}}">
            {% if cdn.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}" alt=""/>
            {% else if cdn.ico %}
              <img src="{{cdn.ico}}" alt=""/>
            {% endif %}
          </a>
        {% endfor %}
        {% if package.github_user and package.github_repo %}
          <a target="_blank" href="https://github.com/{{package.github_user}}/{{package.github_repo}}">
            <img src="{{site.storageUrl.favicon}}/github.ico" alt="">
          </a>
        {% endif %}
        {% if package.storageIco or package.ico and package.homepage %}
          <a target="_blank" href="{{package.homepage}}">
            {% if package.storageIco %}
              <img src="{{site.storageUrl.favicon}}/{{package.storageIco}}" alt=""/>
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
    {% endif %}
  {% endfor %}
</ul>
{% endif %}
