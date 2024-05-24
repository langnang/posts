---
layout: default
title: Home
created_at: 2024-05-15 13:45:58

defaults:
 - scope:
     path:
 - values:
     ico: holder.js/60x60 
links:
 - name: Application
   nameCn: 应用
   url: ./applications/
 - name: Softwares
   nameCn: 程序
   url: ./../softwares/
   target: _blank
 - name: Websites
   nameCn: 网站
   url: ./websites/
 - name: Awesome
   nameCn: 资源推荐
   url: ./awesome/
 - name: CheatSheet
   nameCn: 速查表
   url: ./cheatsheet/
 - name: Guide
   nameCn: 指导
   url: ./guide/
 - name: Question
   nameCn: 试题
   url: ./question/
   visible: false
 - name: Dependencies
   nameCn: 依赖
   url: ./dependencies/
 - name: Standards
   nameCn: 标准规范
   url: ./standards/
 - name: Frameworks
   nameCn: 框架
   url: ./../frameworks/
   target: _blank
   visible: false
 - name: Templates
   nameCn: 模板
   url: ./../templates/
   target: _blank
   visible: false
 - name: Examples
   nameCn: 示例
   url: ./../examples/
   target: _blank
   visible: false 
 - name: Extensions
   nameCn: 拓展
   url: ./../extensions/
   target: _blank
   visible: false  
 - name: Projects
   nameCn: 项目
   url: ./../projects/
   target: _blank
   visible: false   
 - name: Packages
   nameCn: 依赖包
   url: ./../packages/
   target: _blank
   visible: false   
 - name: Games
   nameCn: 游戏
   url: ./../games/
   target: _blank
   visible: false

 - name: 
   nameCn: 
   url: 
   target: 
   visible: 
---

<!-- - [Applications](./applications/): 应用
- [Awesome](./awesome/): 资源列表
- [CheatSheet](./cheatsheet/): 速查表
- [Softwares](./softwares/): 程序
- [Websites](./websites/): 网站
- [SVG](./svg.md)
- [ICO](./ico.md)
- [Emoji](./emoji.md) -->
<style>
    .media>img{
        /* display:none; */
    }
</style>
<div class="container">
  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3">
    {% for link in page.links %}
      {% if link.name and link.visible != false %}
      <div class="col p-2">
          <a class="card" href="{{link.url}}" target="{{link.target}}">
              <div class="card-body p-3">
                  <div class="media">
                      <img src="holder.js/60x60" class="align-self-center mr-2" alt="...">
                      <div class="media-body">
                          <h3 class="card-title mt-0">{{link.name}}</h3>
                          <p class="card-text mb-0">{{link.nameCn}}</p>
                      </div>
                  </div>
              </div>
          </a>
      </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

{% gist ab8ce66b0cada4ecb75a20ec67d481a8 package.json %}
