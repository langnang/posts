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
 - name: Applications
   nameCn: 应用
   url: ./applications
   description: 指手机和电脑的应用。在面向对象上通常分为个人用户应用与企业级应用，在移动端系统分类上主要包括iOS、Android和windows phone的xap和appx。
 - name: Softwares
   nameCn: 程序
   url: ./../softwares/
   target: _blank
   description: 指一组计算机能识别和执行的指令，运行于电子计算机上，满足人们某种需求的信息化工具
 - name: Frameworks
   nameCn: 框架
   url: ./../frameworks/
   target: _blank
   description: 指用于承载一个系统必要功能的基础要素的集合
 - name: Examples
   nameCn: 范例
   url: ./../examples/
   target: _blank
   description: 指可以仿效、典范的事例
 - name: Websites
   nameCn: 网站
   url: ./websites/
   description: 
 - name: Awesome
   nameCn: 资源推荐
   url: ./../awesome/
   target: _blank
   description: 
 - name: CheatSheet
   nameCn: 速查表
   url: ./../cheatsheet/
   description: 指一种为特定领域提供快速查阅所需资料的工具
   target: _blank
 - name: Guide
   nameCn: 指南
   url: ./guide/
   description: 
 - name: Algorithm
   nameCn: 算法
   url: ./../algorithm/
   target: _blank
   description: 
 - name: Interview
   nameCn: 试题
   url: ./../interview/
   target: _blank
   description: 
 - name: Dependencies
   nameCn: 依赖
   url: ./dependencies/
   description: 指程序包运行所需的依赖环境
 - name: Standards
   nameCn: 标准规范
   url: ./standards/
   description: 指某一工程作业或者行为进行定性的信息规定，主要是因为无法精准定量而形成的标准
 - name: Roadmap
   nameCn: 路线规划
   url: ./roadmap/
   description: 指为实现某一目标而进行的有序安排和规划
 - name: Operating System
   nameCn: 操作系统
   url: ./operating-system/
   visible: false
   description: 
 - name: Templates
   nameCn: 模板
   url: ./../templates/
   target: _blank
   description: 指作图或设计方案的固定格式
 - name: Extensions
   nameCn: 拓展
   url: ./../extensions/
   target: _blank
   visible: false  
   description: 指在原有的基础上，增加新的东西。是质量的变化，而不是数量的变化
 - name: Projects
   nameCn: 项目
   url: ./../projects/
   target: _blank
   description: 指进行一项独立一次性或长期无限期的工作任务，以期达到由数量和质量指标所限定的目标
 - name: Packages
   nameCn: 依赖包
   url: ./../packages/
   target: _blank
   visible: false   
   description: 指程序包运行所需的依赖环境
 - name: Games
   nameCn: 游戏
   url: ./../games/
   target: _blank
   visible: false
   description: 指劳作后的休息和消遣，本身不带有任何目的性的一种行为活动
 - name: Feature
   nameCn: 特性
   url: ./../feature/
   target: _blank
   visible: false
   description: 指某事物所特有或特殊的品性、品质
 - name: Mechanism
   nameCn: 机制
   url: ./../mechanism/
   target: _blank
   visible: false
   description: 指各要素之间的结构关系和运行方式
 - name: Ability
   nameCn: 功能
   url: ./../ability/
   target: _blank
   visible: false
   description: 指事物或方法所发挥的有利作用
 - name: PublicAPIs
   nameCn: 公共接口
   url: ./../public-apis/
   target: _blank
   description: 
 - name: Planning
   nameCn: 规划
   url: ./../planning/
   target: _blank
   visible: false
   description: 指个人或组织制定的比较全面长远的发展计划，是对未来整体性、长期性、基本性问题的思考和考量，设计未来整套行动的方案
 - name: Langnang
   nameCn: Langnang
   url: ./../langnang/
   target: _blank
   visible: false
   description: 自研
 - name: # 名称
   nameCn: 
   url: #
   target: # 超链接打开方式 
   visible: #
   description: # 描述
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

- [应用·Application](./application/)
- 软件·Software
- 框架·Framework
- 模板·Template
- 范例·Example
- 推荐·Awesome
- 规范·Standard
- [算法·Algorithm](./algorithm/)
- 试题·Question
- [依赖·Dependency](./dependency/)
- [编程·Program](./program/)

<div class="container d-none">
  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3" style="margin-left: -23px;margin-right: -23px">
    {% for link in page.links %}
      {% if link.name and link.visible != false %}
      <div class="col p-2">
          <a class="card text-decoration-none" href="{{link.url}}" target="{{link.target}}">
              <div class="card-body p-3">
                  <div class="media">
                      <!-- <img src="holder.js/60x60" class="align-self-center mr-2" alt="..."> -->
                      <div class="media-body">
                          <h3 class="card-title mt-0 mb-1">{{link.nameCn}}（{{link.name}}）</h3>
                            {% if link.description %}
                              <p class="card-text text-wrap text-truncate text-muted mb-0" style="height: 3.2rem;display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical;" title="{{link.description}}"> {{link.description}} </p>
                            {% else %}
                              <p class="card-text text-wrap text-truncate text-muted mb-0" style="height: 3.2rem;display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical;" title="{{link.nameCn}}"> {{link.nameCn}} </p>
                            {% endif %}
                      </div>
                  </div>
              </div>
          </a>
      </div>
      {% endif %}
    {% endfor %}
  </div>
</div>

<!-- {% gist ab8ce66b0cada4ecb75a20ec67d481a8 package.json %} -->

<!--
```sh
docs
  ├─ applications     # 应用
  ├─ frameworks       # 框架
  ├─ softwares        # 软件
  ├─ extesions        # 拓展
  ├─ examples         # 范例
  ├─ templates        # 模板
  ├─ packages         # 包裹
  ├─ tools            # 工具
  ├─ games            # 游戏
  └─ projects         # 项目
    ├─ website
    ├─ cheatsheet
    ├─ awesome
    └─ roadmap      
```
-->