---
title: Interview
---
## 前端系列

### HTML

{% if site.data.interview.html_questions %}
{% assign html_questions = site.data.interview.html_questions | slice:0,10 %}
<ul>
  {% for question in html_questions  %}
  <li>{{question.title}}</li>
  {% endfor %}
</ul>
{% endif %}

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./html/">阅读更多</a>

### CSS

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./css/">阅读更多</a>

### JavaScript

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./javascript/">阅读更多</a>

### ECMAScri

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./ecmacript/">阅读更多</a>

### Ajax

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./ajax/">阅读更多</a>

### Vue

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./vue/">阅读更多</a>

### React

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./react/">阅读更多</a>

### TypeScript

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./typescript/">阅读更多</a>

### jQuery

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./jquery/">阅读更多</a>

### NodeJs

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./nodejs/">阅读更多</a>

### 网络&安全防护

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./network-and-security/">阅读更多</a>

### 浏览器

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./chrome/">阅读更多</a>

### 兼容性问题

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./compatibility/">阅读更多</a>

### 性能优化

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./optimize/">阅读更多</a>

### 设计模式

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./design-patterns/">阅读更多</a>

### 工程化

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./engineering/">阅读更多</a>

### 其它未归类

1. 谈谈你对 webpack 的看法（webpack 的特点）
2. 最具有挑战性的项目
3. webpack plugin/loader 的区别
4. 熟悉哪些前端框架并应用于实际项目？ 阅读过哪些前端框架源码并学到哪些？
5. 写过哪些前端组件
6. 前端组件化的理解
7. 有没有写过框架
8. 网站性能优化
9. React/Vue/小程序 的语法的这些好处，坏处
10. Webpack 的代码分割，异步加载资源文件
11. Node Proxy 代理服务, 如何把请求指向本地
12. 如何对网站文件和资源优化
13. 从零写一个 npm 安装包
14. 平时如何管理你的项目？
15. Webpack 中如何配置 Babel
16. promise 和 await/async 的区别是什么？
17. 怎么提高首屏加载速度
18. 模块化开发怎么做？
19. 调试工具的使用
20. 用过哪些设计模式？
21. 简述 gulp 是什么？
22. 列举前端优化策略
23. 首屏、白屏时间如何计算？
24. 如何利用 webpack 把代码上传服务器以及转码测试？
25. 项目上线流程是怎样的？
26. 工程化怎么管理的?
27. webpack 和 gulp 对比 webpack 打包文件太大怎么办?
28. 不想让别人盗用你的图片，访问你的服务器资源该怎么处理？
29. webpack 怎么引入第三方的库？
30. 如果线上出现 bug git 怎么操作？
31. 用过 Nginx 吗？都用过哪些？
32. 混合开发桥接 api 是怎么调用的，需要引入类库嘛? 调用的对象是什么?
33. 说一下你对支付，推送（远程，本地）的理解
34. 后台管理项目，菜单权限如何控制的？
35. 如何调用原生的接口？
36. 微信支付怎么做？说说流程
37. 混合开发的注意点
38. 说说你对手机平台的安装包后缀的理解
39. 谈谈你对 Socket 编程的理解，及实现原理，Socket 之间是怎么通讯的
40. WEB 应用从服务器主动推送 Data 到客户端有哪些方式?
41. 你们原来公司如何发送的新消息推送？
42. webpack 用法
43. 项目开发经历了哪几个阶段
44. WEB 应用从服务器主动推送 Data 到客户端有那些方式？
45. 模块化怎么做？
46. 简述一下你对 web 性能优化的方案
47. 移动端性能优化
48. 请简要描述 web 前端性能需要考虑哪方面，你的优化思路是什么？
49. 业界常用的优化 WEB 页面加载速度的方法（可以分别从页面元素展现，请求连接，css, js, 服务器等方面介绍）
50. 什么是响应式设计？
51. 前端异常监控
52. Ascii、GBK、UTF、Unicode
53. 页面大量图片，如何优化加载，优化用户体验
54. 渲染优化
55. 什么是“前端路由"? 什么时候适合使用“前端路由"? “前端路由"有哪些优点和缺点?
56. 前端项目监控怎么做的
57. 前后端分离的项目如何seo
58. 怎么判断页面是否加载完成？
59. 垃圾回收 新生代算法，老生代算法
60. 介绍MVP怎么组织（宝宝树）
61. 如何实现骨架屏，说说你的思路
62. 如何在 H5 和小程序项目中计算白屏时间和首屏时间，说说你的思路
63. 前端项目如何找出性能瓶颈（阿里）
64. 介绍下 npm 模块安装机制，为什么输入 npm install 就可以自动安装对应的模块？
65. 观察者和订阅-发布的区别，各自用在哪里（网易）
66. 文件上传如何做断点续传（网易）
67. npm2和npm3 有什么区别(宝宝树)
68. 移动端如何设计一个比较友好的Header组件？(携程)
69. 说说你对前端架构师的理解
70. 你如何对需求原型进行理解和拆分
71. 说说你对功能性需求的理解
72. 说说你对非功能性需求的理解
73. 你针对产品提出哪些交互和改进意见
74. 你如何理解用户痛点
75. 说说你在项目中使用过的UML 图
76. 你如何考虑组件化
77. 你如何考虑服务化
78. 你如何进行领域建模
79. 你如何划分领域边界
80. 说说你项目中的领域建模
81. 说说概要设计
82. 你使用过哪些设计模式，请介绍一下分别使用场景以及它们自身
83. 说说常用开源框架中设计模式使用分析
84. 说说你对设计原则的理解23种设计模式的设计理念
85. 设计模式之间的异同，例如策略模式与状态模式的区别
86. 设计模式之间的结合，例如策略模式 + 简单工厂模式的实践
87. 设计模式的性能，例如单例模式哪种性能更好。
88. 你系统中的前后端分离是如何做的
89. 说说你的开发流程
90. 你和团队是如何沟通的
91. 你如何进行代码评审
92. 说说你对技术与业务的理解
93. 说说你在项目中经常遇到的 Exception
94. 说说你在项目中遇到感觉最难 Bug，怎么解决的
95. 说说你在项目中遇到印象最深，最困难的地方，是怎么解决的
96. 你觉得你们项目还有哪些不足的地方
97. 你是否遇到过 CPU 100%，如何排查与解决
98. 你是否遇到过 内存 OOM，如何排查与解决
99. 说说你对敏捷开发的实践
100. 说说你对开发运维的实践
101. 介绍下工作中的一个对自己最有价值的项目，以及在这个过程中的角色
102. 为什么通常在发送数据埋点请求的时候使用的是 1x1 像素的透明 gif 图片？
103. 在前后端分离项目里，请说说前端传递的token的流程？
104. 你觉得新开发一个网站最困难的是哪些部分？
105. 前端打包工具rollup、webpack、vite的区别
106. 如何实现快速冷启动？
107. npm打包时需要注意哪些？如何利用webpack来更好的构建？

## 服务端系列

### PHP

## 算法系列

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./algorithm/">阅读更多</a>

## LeetCode

<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./leetcode/">阅读更多</a>

## References
<!--
- [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/user/repo)
    ![](https://img.shields.io/github/stars/?style=flat)
      user/repo:
 -->
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/0voice/interview_internal_reference)
    ![](https://img.shields.io/github/stars/0voice/interview_internal_reference?style=flat)
    `0voice/interview_internal_reference`:
        2023 年最新总结，阿里，腾讯，百度，美团，头条等技术面试题目，以及答案，专家出题人分析汇总。
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/doocs/leetcode)
    ![](https://img.shields.io/github/stars/doocs/leetcode?style=flat)
    `doocs/leetcode`:
        🔥LeetCode solutions in any programming language | 多种编程语言实现 LeetCode、《剑指 Offer（第 2 版）》、《程序员面试金典（第 6 版）》题解
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/Advanced-Frontend/Daily-Interview-Question)
    ![](https://img.shields.io/github/stars/Advanced-Frontend/Daily-Interview-Question?style=flat)
    [![](https://muyiy.cn/favicon.ico)](https://muyiy.cn/question/)
    `Advanced-Frontend/Daily-Interview-Question`:
        我是依扬（木易杨），公众号「高级前端进阶」作者，每天搞定一道前端大厂面试题，祝大家天天进步，一年后会看到不一样的自己。
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/haizlin/fe-interview)
    ![](https://img.shields.io/github/stars/haizlin/fe-interview?style=flat)
    `haizlin/fe-interview`:
        前端面试每日 3+1，以面试题来驱动学习，提倡每日学习与思考，每天进步一点！每天早上 5 点纯手工发布面试题（死磕自己，愉悦大家），6000+道前端面试题全面覆盖，HTML/CSS/JavaScript/Vue/React/Nodejs/TypeScript/ECMAScritpt/Webpack/Jquery/小程序/软技能……
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/febobo/web-interview)
    ![](https://img.shields.io/github/stars/febobo/web-interview?style=flat)
    `febobo/web-interview`:
        语音打卡社群维护的前端面试题库，包含不限于 Vue 面试题，React 面试题，JS 面试题，HTTP 面试题，工程化面试题，CSS 面试题，算法面试题，大厂面试题，高频面试题
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/wolverinn/Waking-Up)
    ![](https://img.shields.io/github/stars/wolverinn/Waking-Up?style=flat)
    `wolverinn/Waking-Up`:
        计算机基础（计算机网络/操作系统/数据库/Git...）面试问题全面总结，包含详细的follow-up question以及答案
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/yuanguangxin/LeetCode)
    ![](https://img.shields.io/github/stars/yuanguangxin/LeetCode?style=flat)
    `yuanguangxin/LeetCode`:
        LeetCode 刷题记录与面试整理
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/lgwebdream/FE-Interview)
    ![](https://img.shields.io/github/stars/lgwebdream/FE-Interview?style=flat)
    [![](https://lgwebdream.github.io/FE-Interview/img/favicon.ico)](https://lgwebdream.github.io/FE-Interview/)
    `lgwebdream/FE-Interview`:
        🔥🔥🔥 前端面试，独有前端面试题详解，前端面试刷题必备，1000+前端面试真题，Html、Css、JavaScript、Vue、React、Node、TypeScript、Webpack、算法、网络与安全、浏览器
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/paddingme/Front-end-Web-Development-Interview-Question)
    ![](https://img.shields.io/github/stars/paddingme/Front-end-Web-Development-Interview-Question?style=flat)
    `paddingme/Front-end-Web-Development-Interview-Question`:
        前端开发面试题大收集，前端面试集锦 ❤️ 💝 💘
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/yangchong211/YCBlogs)
    ![](https://img.shields.io/github/stars/yangchong211/YCBlogs?style=flat)
   `yangchong211/YCBlogs`:
        技术博客笔记大汇总，包括Java基础，线程，并发，数据结构；Android技术博客等等；常用设计模式；常见的算法；网络协议知识点；部分flutter笔记；还包括平时开发中遇到的bug汇总，当然也在工作之余收集了大量的面试题，长期更新维护并且修正，持续完善……
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/shfshanyue/Daily-Question)
    ![](https://img.shields.io/github/stars/shfshanyue/Daily-Question?style=flat)
    `shfshanyue/Daily-Question`:
        互联网大厂内推及大厂面经整理，并且每天一道面试题推送。每天五分钟，半年大厂中
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/itcharge/LeetCode-Py)
    ![](https://img.shields.io/github/stars/itcharge/LeetCode-Py?style=flat)
    `itcharge/LeetCode-Py`:
        ⛽️「算法通关手册」：超详细的「算法与数据结构」基础讲解教程，从零基础开始学习算法知识，850+ 道「LeetCode 题目」详细解析，200 道「大厂面试热门题目」。
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/jirengu/frontend-interview)
    ![](https://img.shields.io/github/stars/jirengu/frontend-interview?style=flat)
    `jirengu/frontend-interview`:
        前端笔试面试题题库
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/yisainan/web-interview)
    ![](https://img.shields.io/github/stars/yisainan/web-interview?style=flat)
    `yisainan/web-interview`:
        我是齐丶先丶森，收集整理全网面试题及面试技巧，旨在帮助前端工程师们找到一份好工作！
[**interview · GitHub Topics**](https://github.com/topics/interview)
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/jwasham/coding-interview-university)
    ![](https://img.shields.io/github/stars/jwasham/coding-interview-university?style=flat)
        jwasham/coding-interview-university:
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/donnemartin/system-design-primer)
    ![](https://img.shields.io/github/stars/donnemartin/system-design-primer?style=flat)
        donnemartin/system-design-primer
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/trekhleb/javascript-algorithms)
    ![](https://img.shields.io/github/stars/trekhleb/javascript-algorithms?style=flat)
      trekhleb/javascript-algorithms
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/TheAlgorithms/Python)
    ![](https://img.shields.io/github/stars/TheAlgorithms/Python?style=flat)
      TheAlgorithms/Python
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/CyC2018/CS-Notes)
    ![](https://img.shields.io/github/stars/CyC2018/CS-Notes?style=flat)
      CyC2018/CS-Notes
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/Snailclimb/JavaGuide)
    ![](https://img.shields.io/github/stars/Snailclimb/JavaGuide?style=flat)
      Snailclimb/JavaGuide
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/bregman-arie/devops-exercises)
    ![](https://img.shields.io/github/stars/bregman-arie/devops-exercises?style=flat)
      bregman-arie/devops-exercises
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/kdn251/interviews)
    ![](https://img.shields.io/github/stars/kdn251/interviews?style=flat)
      kdn251/interviews
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/azl397985856/leetcode)
    ![](https://img.shields.io/github/stars/azl397985856/leetcode?style=flat)
      azl397985856/leetcode
* [![]({{site.storageUrl.favicon}}/github.ico)]({{site.siteUrl.github}}/binhnguyennus/awesome-scalability)
    ![](https://img.shields.io/github/stars/binhnguyennus/awesome-scalability?style=flat)
      binhnguyennus/awesome-scalability
