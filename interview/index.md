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

### ECMAScri<a class="alert alert-primary small text-center d-block py-1" role="alert" href="./ecmacript/">阅读更多</a>

### Ajax

### Vue

### React

### TypeScript

### jQuery

### NodeJs

### 网络&安全防护

1. Http 状态码，Http2 是什么
2. http1. 1 时如何复用 tcp 连接（网易）
3. Http 请求的整个过程
4. http 缓存配置怎么设置
5. 常见的浏览器端的存储技术有哪些， 以及它们的优缺点和使用场景？
6. 在 HTTP 响应 Header 中，set-cookie 选项有哪些，分别代表什么含义？
7. 何为跨域？ 跨域请求数据有几种方式？图片/脚本 等资源有什么跨域问题。如何解决？跨域请求时如何携带 cookie
8. 简要描述 HTTPS 的安全机制，以及在 web 服务工程实践中需要注意的问题。描述 http2 和 https 的关系
9. 什么是点击劫持？如何防范？
10. 什么是 CSRF, 怎么造成的，有什么防御方法？
11. 请简述如何在 HTML 中开启和关闭 DNS 预读取?
12. 什么是回源？域名回源的含义是什么？
13. https 实现原理
14. HTML5 的离线储存怎么使用，工作原理能不能解释一下
15. XSS
16. CSRF cookie 问题？
17. CDN 原理
18. 如何启动浏览器硬件加速，小 Hack
19. 什么是 Cookie 隔离？（或者说：请求资源的时候不要让它带 cookie 怎么做）
20. 三次握手
21. 四次挥手
22. 线程与进程的区别
23. WEB 应用从服务器主动推送 Data 到客户端有那些方式？
24. HTTP 的几种请求方法用途
25. 常见 web 安全及防护原理
26. 为什么要有同源限制？
27. 域名发散和域名收敛是什么？
28. 什么是 HTTPS，做什么用的呢？如何开启 HTTPS？
29. TCP 和 UDP 的区别
30. Web Worker 和 webSocket
31. 为什么 HTTPS 安全
32. sql 注入原理
33. XSS 原理及防范
34. XSS 防范方法
35. XSS 与 CSRF 有什么区别吗？
36. CSRF 的防御
37. 请你谈谈 Cookie 的弊端？
38. HTTP 协议中，header 信息里面，怎么控制页面失效时间（last-modified, cache-control, Expires 分别代表什么）
39. 本地存储（Local Storage ）和 cookies（储存在用户本地终端上的数据）之间的区别是什么？
40. Accept 和 Content-Type
41. http 协议缓存机制
42. 如何处理不让别人盗用你的图片，访问你的服务器资源
43. Http 与 Https 的区别
44. 什么是 Http 协议无状态协议? 怎么解决 Http 协议无状态协议?
45. 常用的 HTTP 方法有哪些
46. 一次完整的 HTTP 请求所经历的 7 个步骤
47. webSocket 如何兼容低版本浏览器？
48. 介绍 SSL 和 TLS（寺库）
49. 说说网络的五层模型（寺库）
50. cookie 和 token 都存放在 header 中，为什么不会劫持 token？
51. v8 有了解过吗？讲讲了解过 v8 的那几个模块和部分，比如解释一下 v8 的 hidden class
52. 前端如何实现即时通讯？
53. Http 状态码 301 和 302 的应用场景分别是什么
54. 接口如何防刷
55. 为什么 HTTP1. 1 不能实现多路复用
56. HTTPS 握手过程中，客户端如何验证证书的合法性
57. 介绍 HTTPS 握手过程
58. 简单讲解一下 http2 的多路复用
59. HTTP2.  0 的多路复用和 HTTP1.  X 中的长连接复用区别
60. 单工、半双工和全双工的区别
61. 长连接与短连接
62. 应用层--HTTP 协议
63. 应用层--HTTP/2 协议
64. 应用层--HTTPS 协议
65. 应用层--DNS 协议
66. 传输层--多路复用与多路分解
67. 传输层--UDP 协议
68. 传输层--TCP 协议
69. 网络层
70. 数据链路层
71. 物理层
72. TLS/SSL 中什么一定要用三个随机数，来生成"会话密钥"？
73. SSL 连接断开后如何恢复？
74. RSA 算法的安全性保障？
75. DNS 为什么使用 UDP 协议作为传输层协议？
76. 当你在浏览器中输入 Google.com 并且按下回车之后发生了什么？
77. 谈谈 CDN 服务？
78. 什么是正向代理和反向代理？
79. 负载平衡的两种实现方式？
80. http 请求方法 options 方法有什么用？
81. http1. 1 和 http1. 0 之间有哪些区别？
82. 网站域名加 www 与不加 www 的区别？
83. 即时通讯的实现，短轮询、长轮询、SSE 和 WebSocket 间的区别？
84. 怎么实现多个网站之间共享登录状态
85. token相对cookie的优势
86. JWT是什么
87. Cookie、Session、Token、JWT对比与总结
88. http中的301、302、307、308有什么区别？
89. 说说你对短连接的理解，它有什么应用场景呢？
90. 列举你所了解的计算机存储设备类型？
91. web安全:平行越权和垂直越权

### 浏览器

### 兼容性问题


### 性能优化

### 设计模式

### 工程化

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

* 排序
  * 冒泡排序
选择排序
插入排序
希尔排序
归并排序
快速排序
堆排序
基数排序
快速排序相对于其他排序效率更高的原因
系统自带排序实现
稳定性
排序面试题目总结
树
二叉树相关性质
满二叉树
完全二叉树
平衡二叉查找树（AVL）
B-树
B+树
数据库索引
红黑树
Huffman 树
二叉查找树
求解二叉树中两个节点的最近公共祖先节点
链表
反转单向链表
动态规划
爬楼梯问题
递归方法分析
备忘录方法
迭代法
经典笔试题

1. js 实现一个函数，完成超过范围的两个大整数相加功能
2. js 如何实现数组扁平化？
3. js 如何实现数组去重？
4. 如何求数组的最大值和最小值？
5. 如何求两个数的最大公约数？
6. 如何求两个数的最小公倍数？
7. 实现 IndexOf 方法？
8. 判断一个字符串是否为回文字符串？
9. 实现一个累加函数的功能比如 sum(1,2,3)(2).valueOf()
10. 使用 reduce 方法实现 forEach、map、filter
11. 设计一个简单的任务队列，要求分别在 1,3,4 秒后打印出 "1", "2", "3"
12. 如何查找一篇英文文章中出现频率最高的单词？
常见面试智力题总结 - 1.  时针与分针夹角度数问题？ - 2.   用3升，5升杯子怎么量出4升水？ - 3.  四个药罐中有一个浑浊的药罐，浑浊的每片药片都比其他三个干净的药罐多一克，如何只用一次天平找出浑浊的药罐？ - 4.  四张卡片，卡片正面是数字，反面是字母。现在桌上四张卡片，状态为 a 1 b 2 现在我想要证明 a 的反面必然是 1 ，我只能翻两张牌，我翻哪两张？ - 5.  赛马问题，25 匹马，5 个赛道，最少几次能选出最快的三匹马？ - 6.  五队夫妇参加聚会，每个人不能和自己的配偶握手，只能最多和他人握手一次。A问了其他人，发现每个人的握手次数都不同，那么A的配偶握手了几次？ - 7.  你只能带行走 60 公里的油，只能在起始点加油，如何穿过 80 公里的沙漠？ - 8.  烧一根不均匀的绳要用一个小时，如何用它来判断一个小时十五分钟？ - 9.  有7克、2克砝码各一个，天平一只，如何只用这些物品三次将140克的盐分成50、90克各一份？ - 10.  有一辆火车以每小时15公里的速度离开洛杉矶直奔纽约，另一辆火车以第 小时20公里的速度从纽约开往洛杉矶。如果有一只鸟，以外30公里每小时的速度和 两辆火车现时启动，从洛杉矶出发，碰到另辆车后返回，依次在两辆火车来回的飞行，直道两面辆火车相遇，请问，这只小鸟飞行了多长距离？ - 11.  你有两个罐子，50个红色弹球，50个蓝色弹球，随机选出一个罐子，随机选取出一个弹球放入罐子，怎么给红色弹球最大的选中机会？在你的计划中，得到红球的准确几率是多少？ - 12.   假设你有8个球，其中一个略微重一些，但是找出这个球的惟一方法是将两个球放在天平上对比。最少要称多少次才能找出这个较重的球？ - 13.  在房里有三盏灯，房外有三个开关，在房外看不见房内的情况，你只能进门一次，你用什么方法来区分那个开关控制那一盏灯？ - 14.  他们都各自买了两对黑袜和两对白袜，八对袜子的布质、大小完全相同，而每对袜子都有一张商标纸连着。两位盲人不小心将八对袜子混在一起。他们每人怎样才能取回黑袜和白袜各两对呢？ - 15.  有三筐水果，一筐装的全是苹果，第二筐装的全是橘子，第三筐是橘子与苹果混在一起。筐上的标签都是骗人的，（就是说筐上的标签都是错的）你的任务是拿出其中一筐，从里面只拿一只水果，然后正确写出三筐水果的标签。 - 16.  一个班级60%喜欢足球，70%喜欢篮球，80%喜欢排球，问即三种球都喜欢占比有多少？ - 17.  五只鸡五天能下五个蛋，一百天下一百个蛋需要多少只鸡？
剑指 offer 思路总结
题目
1. 二维数组中的查找
2. 替换空格
3. 从尾到头打印链表
4. 重建二叉树
5. 用两个栈实现队列
6. 旋转数组的最小数字
7. 斐波那契数列
8. 跳台阶
9. 变态跳台阶
10. 矩形覆盖
11. 二进制中1的个数
12. 数值的整数次方
13. 调整数组顺序使奇数位于偶数前面
14. 链表中倒数第 k 个节点
15. 反转链表
16. 合并两个排序的链表
17. 树的子结构
18. 二叉树的镜像
19. 顺时针打印矩阵
20. 定义一个栈，实现 min 函数
21. 栈的压入弹出
22. 从上往下打印二叉树
23. 二叉搜索树的后序遍历
24. 二叉树中和为某一值路径
25. 复杂链表的复制
26. 二叉搜索树与双向链表
27. 字符串的排列
28. 数组中出现次数超过一半的数字
29. 最小的 K 个数
30. 连续子数组的最大和
31. 整数中1出现的次数（待深入理解）
32. 把数组排成最小的数
33. 丑数（待深入理解）
34. 第一个只出现一次的字符
35. 数组中的逆序对
36. 两个链表的第一个公共结点
37. 数字在排序数组中出现的次数
38. 二叉树的深度
39. 平衡二叉树
40. 数组中只出现一次的数字
41. 和为 S 的连续正数序列
42. 和为 S 的两个数字
43. 左旋转字符串
44. 翻转单词顺序列
45. 扑克牌的顺子
46. 圆圈中最后剩下的数字（约瑟夫环问题）
47. 1+2+3+...+n
48. 不用加减乘除做加法
49. 把字符串转换成整数。
50. 数组中重复的数字
51. 构建乘积数组
52. 正则表达式的匹配
53. 表示数值的字符串
54. 字符流中第一个不重复的字符
55. 链表中环的入口结点
56. 删除链表中重复的结点
57. 二叉树的下一个结点
58. 对称二叉树
59. 按之字形顺序打印二叉树（待深入理解）
60. 从上到下按层打印二叉树，同一层结点从左至右输出。每一层输出一行。
61. 序列化二叉树（待深入理解）
62. 二叉搜索树的第 K 个节点
63. 数据流中的中位数（待深入理解）
64. 滑动窗口中的最大值（待深入理解）
65. 矩阵中的路径（待深入理解）
66. 机器人的运动范围（待深入理解）
相关算法题
1. 明星问题
2. 正负数组求和

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
