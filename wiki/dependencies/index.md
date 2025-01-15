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




---



<div class="d-flex justify-content-around mb-3" style="height: 3rem;">
  {% for cdn in page.cdns %}
    <a target="_blank" class="d-inline-flex" href="{{cdn.homepage}}" title="{{cdn.name}}">
      {% if cdn.storageIco %}
        <img src="{{site.storageUrl.favicon}}/{{cdn.storageIco}}"/>
      {% else if cdn.ico %}
        <img src="{{cdn.ico}}"/>
      {% endif %}
    </a>
  {% endfor %}
</div>

- [NPM](./npm/)
- [Composer](./composer.md)
- [Ruby](./ruby.md)
- [PyPI](./pipy.md)
