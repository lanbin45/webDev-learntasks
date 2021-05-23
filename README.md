# webDev-learntasks

# 0. 本机开发必备工具

1. chrome，建议添加“彩云小译”扩展，用于英文文档的中英文对照阅读
1. vscode
1. git
1. nodejs

## 要求

1. 学习之前创建一个 github 账号，新建一个 repo，每天以 markdown 格式文件，按日期命名完成以下两个部分内容：
   - **学习笔记**： 记录你每天学习过程中认为有用处的学习笔记；
   - **每日学习总结**: 每天学习完毕，多花十分钟，总结自己的笔记，整理自己的学习思路，巩固记忆。 `此项每天检查`
   - **练习项目的代码**: 后续学习中对应的项目代码整理归档；

有以下几个目的:

- 督促学习；
- 联系 git 代码使用，所以代码和 md 文件提交尽量使用命令行模式；
- 学习 markdown 语法；
- 总结回顾每日学习的内容，整理思路

## 参考资料和教程

以下教程仅供环境配置参考，能配置开发环境即可，后续使用时，不会的命令可以以此作为备查

1. vscode 使用教程: https://zhuanlan.zhihu.com/p/113222681
1. git 使用教程: http://xqdoc.imedao.com/1533b6a26a1124b3fe570db9.pdf
1. node 推荐使用版本管理工具:
   - nvm (windows): https://www.jianshu.com/p/24371f85c832
   - n (mac): https://www.jianshu.com/p/a52bb03cb279
1. node 包管理工具推荐使用 yarn https://yarnpkg.com/
1. markdown 语法教程: https://www.markdown.xyz/basic-syntax/
1. 免费梯子工具, 需要请自取: https://ikuuu.org/auth/register?code=2gdh
1. vue-devtools 开发插件: https://chrome.pictureknow.com/extension?id=d50143a5f53d406dbe992277bfc90521
1. @vue/cli-service: https://cli.vuejs.org/guide/cli-service.html

> 本文档提供的部分任务和知识点提供 React 和 Vue 两种版本，以 Vue 为主，React 的内容仅列做参考，方便您以后学习，不做考察

# 1. Web 开发基础知识：HTML/CSS/JS

## 任务

使用 HTML 和 CSS，实现以下页面的静态版本：

1. 必应搜索页 https://cn.bing.com/ 和搜索结果页 https://cn.bing.com/search?q=html+css
1. vuejs 网站首页 https://vuejs.org/ 和团队介绍页 https://vuejs.org/v2/guide/team.html (人员列表显示 5 条即可)
1. 知乎热榜页 https://www.zhihu.com/hot (登录知乎后可见，热榜显示前十条）
1. github issue 列表页 https://github.com/THU-SYU-WebDev/docs/issues 和 issue 编辑页 https://github.com/THU-SYU-WebDev/docs/issues/new （登录 github 后可见）

具体要求:

1. 每一小组选以上四题中一题即可，但不能有多个小组选择同一题目。请各组相互协调选择
1. 只通过 HTML CSS 复刻静态结果页面，不需要用 JS 实现点击跳转、菜单弹出、图片轮播、获取数据等动态功能
1. 与原始页面排版、布局、字体、颜色尽量相似，能做到像素级复原就最好了
1. 尽量使用 `display: flex` 实现页面布局，不要照搬原始页面的 html 和 css 结构。原页面结果大多不是用 flex 的，所以如果照抄原页面的话，很容易看出来的
1. 图片等资源可以从原网页上另存，然后用在你自己的页面里

## 推荐教程和参考文档

1. MDN https://developer.mozilla.org/zh-CN/docs/Learn
1. HTML: https://developer.mozilla.org/zh-CN/docs/Web/HTML/Reference
1. CSS: https://developer.mozilla.org/zh-CN/docs/Web/CSS/Reference
1. JS: 查看过程中，有一些代码可以 f12 打开浏览器控制台
   1. https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps
   1. https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks
   1. https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array
   1. https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object
   1. https://es6.ruanyifeng.com/ （先看 0 - 5, 7 - 11, 16, 21 - 22 章）
1. flex 布局博客可以参考阮一峰的这篇，讲得比较通透: https://www.ruanyifeng.com/blog/2015/07/flex-examples.html

注意事项：

- MDN 是相对最权威、最全面准确、更新最即时的 Web 文档站。尽量不要看百度出来的中文教程，除非特别简单传统的部分如 DOM API 等可以看 w3school 等
- “教程”和“参考”是不一样的，“教程”是面向初学者的，要逐字逐句弄懂；“参考”则是真正开发时的备查手册，初学时无须详细阅读
- 如果有读不太懂的地方，大概率是翻译问题，可以另开一个英文版页面，中英版本对照阅读
- 少数页面还没有中文版本，可使用 chrome 自带的翻译工具、或“彩云小译”翻译插件阅读
- 读文档时，可随时在 vscode 编辑器里实际写一点页面来测试，在 chrome 里看实际效果

## 知识点回顾

1. 从前端经典面试题 `在浏览器输入 URL 回车之后发生了什么` https://juejin.cn/post/6844903922084085773 ，整体理解并串联起前端的重要概念
1. 阮一峰这个 ES6 教程 https://es6.ruanyifeng.com/ 可以多看一下，以后编码中高频使用；
1. 结合一些面试常见问题，重点巩固面试要用的知识,比如： https://segmentfault.com/a/1190000021966814

# 2. web 开发技术演进历史

## 任务

在上次作业基础上，尝试使用历史上的三种主流方法生成动态页面（或三选一）：

1. CGI/ASP/PHP 时代：运用你学过的后端语言的编程能力，动态拼接字符串生成 html 页面，向前端输出动态页面内容;
2. DOM/jQuery 时代：使用 JS DOM API 的动态修改页面能力，在浏览器中“命令式”地生成动态内容；
3. 前端框架时代：使用 Vue/React/Angular 等当代前端框架，在浏览器中“声明式”地生成动态内容。

着重考虑三种”动态能力“：

1. 分支
2. 循环
3. 函数

## 推荐教程和参考文档

1. JS: https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference
1. DOM: https://www.w3school.com.cn/htmldom/index.asp
1. Web API: https://developer.mozilla.org/zh-CN/docs/Web/API
1. Vue 2 官方站: https://cn.vuejs.org/v2/

# 3. 当代前端主流框架入门： 用 React & Vue 实现 Tic Tac Toe 小游戏

## 任务

本次各组任务相同：使用六种不同的技术完成 React 官方教程所示的 Tic Tac Toe 小游戏 （https://codepen.io/gaearon/pen/gWWZgR）：

1. 无论你 JS 基础如何，请按顺序阅读以下 JS 文档，必要的话上手做点小练习：

   1. https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/First_steps
   1. https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Building_blocks
   1. https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array
   1. https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object
   1. https://es6.ruanyifeng.com/ （先看 0~5, 7~11, 16, 21~22 章）

1. 熟悉 DOM API:

   1. https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Client-side_web_APIs/
   1. https://www.w3school.com.cn/htmldom/index.asp

~~1. React 入门~~

1.  阅读 React 官方入门教程 https://zh-hans.reactjs.org/tutorial/tutorial.html, 并根据教程完成 Tic Tac Toe 小游戏（具体做法教程都告诉你了，就是跟着实现一遍）
1.  阅读 React 官方文档 https://zh-hans.reactjs.org/docs/getting-started.html, 按顺序看以下部分： _核心概念_； _高级指引_ 下的 _Context_、_Fragment_、_深入 JSX_、_性能优化_、_协调_、_Refs & DOM_、_非受控组件_；_HOOK_），使用 Hook API 复刻 Tic Tac Toe 小游戏

1.  Vue 入门：

    1.  阅读 Vue 2 官方文档 https://cn.vuejs.org/v2/guide/ 开头的 _基础_ 部分，使用 Vue 复刻 Tic Tac Toe 小游戏
    1.  继续阅读 Vue 2 官方文档 https://cn.vuejs.org/v2/guide/ 的 _深入了解组件_ 和 _可复用 & 组合_ 部分，使用 Vue2 复刻 Tic Tac Toe 小游戏
        ~~1. 阅读 https://github.com/vuejs/jsx-next, 使用 Vue Composition API + JSX 复刻 Tic Tac Toe 小游戏~~

1.  回到 DOM API:
    1.  阅读 React 作者之一 Dan Abramov 的文章 https://overreacted.io/the-bug-o-notation/, 体会前端框架的意义
    1.  不使用任何前端框架，用原生 DOM API 复刻 Tic Tac Toe 小游戏。注意，上面这篇文章表明，即使都是用 DOM API，代码组织水平也有高下之分。在没有框架约束的情况下，请仔细斟酌你的代码结构，尽量提高可读性、可维护性
    1.  对比这几个版本，你认为 Vue 和 React 这样的前端库/框架，和原始的 JS DOM API 相比，带来了什么好处，解决了什么问题？

- 说明：

  - Vue 官方教程写得非常非常好，新版的 React 官方教程 + React 团队成员 Dan Abramov 的技术博客也不错。一般来说不必去学习网上那些收费的文字或视频教程
  - React Function Component + Hooks 已经代替 React Class Component 成为当前全球前端就业热点，hooks 的原理有点反直觉，一定要搞明白

# 4. 当代前端主流框架进阶： 用 React & Vue 实现 ToDoMVC

## 任务

1. 把上节未全部看完的 React & Vue 官方文档全部看完，API 也都浏览一遍，做到心里有大概印象，知道框架有哪些功能，开发实际用到的时候知道在哪里查具体用法（可跳过和测试相关的部分），并书面回答以下问题：

   1. 说说 Vue 和 React 的 API 相似性，比如 React 的 Composition Component、render props、useState、useEffect、useContext，分别对应着 Vue 的哪些概念或 API？
   1. 说说两者 API 的差异性，比如哪些是 React 有而 Vue 没有的，哪些是 Vue 有和 React 没有的？

1. TodoMVC (https://todomvc.com/examples/vanillajs/) 是一个标准的前端视图开发入门项目。与上一个任务类似，这次请使用以下五种技术，复刻五个版本的 TodoMVC。要求界面 css 样式和原版完全一样，但不要求支持浏览器地址栏地址（URL）随操作变化的功能（即不要求有路由功能）。

   这里暂时只要求使用 Vue 2.x，后续感兴趣可以尝试使用以下几种方式实现:

   1. React Class Component API
   1. React Hooks API
   1. Vue 3 Options API + Template
   1. Vue 3 Composition API + Template
   1. Vue 3 Composition API + JSX

1. 深入理解 JS 变量的内存模型、传参方式以及可变性（对正确使用 React 和 Vue 都非常非常重要，不懂的话以后就会经常掉坑）：

   1. https://justjavascript.com/ 从这里可以订阅 Dan Abramov 的一个教学邮件列表，一章一章地阅读并做练习。写得非常非常好。不要怕英语，作者是俄罗斯人，使用的英语很简单很好懂。
   1. https://zhuanlan.zhihu.com/p/62449359
   1. https://segmentfault.com/a/1190000012829900
   1. https://www.zhihu.com/question/51018162
   1. https://dzone.com/articles/immutability-in-javascriptwhy-and-when-should-you

1. 书面回答以下问题：

   1. 结合 JS 变量内存模型分析，JS 中哪些数据类型是 **可变** 的，哪些数据类型是 **不可变** 的？
   1. JS 关于数组和对象的方法和解构语法中，哪些方法和语法会修改原值，哪些不修改原值而是返回新值？
   1. JS 的 `const` 表明了对象 **不可重新赋值**，这和对象、数组的可变性冲突吗？为什么？

1. 深入学习 React 基础原理：

   1. https://overreacted.io/react-as-a-ui-runtime/ （中文版翻译有很多错误，请中英对照阅读）
   1. https://overreacted.io/a-complete-guide-to-useeffect/ （中文版翻译得不太好，请中英对照阅读）

1. 深入学习 Vue 基础原理：

   1. https://es6.ruanyifeng.com/#docs/proxy
   1. https://zhuanlan.zhihu.com/p/330902107 (除了 Proxy 响应原理，还讲了 依赖收集，选读)

1. 根据上述基础原理，结合开发 Tic Tac Toe、TodoMVC 过程中的感受，书面回答以下问题：

   1. 在五个版本中，你为 TodoMVC 这个 app 设计了怎样的数据结构来保存以完成、未完成的 todo 列表信息？（即 Model 层设计）
   1. 在五个版本中，你是遵循怎样的思路把这些 Model 数据转化为页面上显示的内容的？又是怎样把用户在页面上的操作行为转化为对 Model 数据的修改的？（即 Model 层和 View 层的互动）
   1. 你认为 Vue 和 React 的最本质区别是什么？是双向绑定 vs 单向数据流吗？是 template vs JSX 语法吗？是实现数据-视图响应联动的方法不同吗？还是别的什么？请详述。

# 5. 前端路由

## 任务

观察原版 TodoMVC (https://todomvc.com/examples/vanillajs/) 的浏览器地址栏内容（即 URL）是怎么根据用户操作而变化的，浏览器前进后退按钮是怎么配合 URL 工作的，<strike>然后给你自己的以下三个版本 TodoMVC 都加上相应的功能。</strike>，

<strike> 1. React Hooks API </strike>
<strike> 1. 使用 Vue 2.x 和 Vue-router 完成相应功能: 使用传统的 `this.$router` `this.$route` 语法 </strike>

## 推荐教程和参考文档

1. https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/What_is_a_URL
1. https://developer.mozilla.org/zh-CN/docs/Web/API/History_API
1. https://developer.mozilla.org/zh-CN/docs/Web/API/History_API/Working_with_the_History_API
1. React Router: https://reactrouter.com/
1. Vue Router for Vue 3: https://next.router.vuejs.org

# 6. 连接前后端的信使：HTTP 与异步 JS

## 任务

使用 Vue 2.x 为 TodoMVC 添加服务端数据存取功能，做到每次关闭页面重新打开之后数据不消失：

【TODO】将为此任务提供一个公共后端服务地址，一次存取所有 Todo 数据。

## 推荐教程和参考文档

1. HTTP 概述:
   1. https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Overview
   1. https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/How_does_the_Internet_work
   1. https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/Pages_sites_servers_and_search_engines
1. 程序员都该懂点 HTTP: https://juejin.cn/post/6844903511633707021
1. 异步 JS: https://developer.mozilla.org/zh-CN/docs/Learn/JavaScript/Asynchronous
1. 异步 ES6: https://es6.ruanyifeng.com/ (16~20 章）
1. fetch API: https://developer.mozilla.org/zh-CN/docs/Web/API/Fetch_API
1. axios: https://www.npmjs.com/package/axios
1. 使用 React Hook: https://www.robinwieruch.de/react-hooks-fetch-data

# 7. 后端入门：NodeJS Express & Python Flask

## 任务

为两个版本的 TodoMVC 分别自建 http 服务：

1. Vue 2.x: 建立 NodeJS Express 后端框架的 http server
   <strike> 1. Vue 3 Composition API + JSX: 建立 Python Flask 后端框架的 http server </strike>

服务器应提供以下俩两个功能：

1. 静态文件服务：向前端提供 TodoMVC 的 html/css/js 文件
2. 动态数据服务：将 TodoMVC 数据整体存放在后端服务器内存中，接受前端 GET 请求时发送数据，接受前端 POST 请求时更新数据。

## 推荐教程和参考文档

1. 服务器概念：https://developer.mozilla.org/zh-CN/docs/Learn/Common_questions/What_is_a_web_server
1. flask 文档：https://dormousehole.readthedocs.io/en/latest/index.html
1. express 文档：https://www.expressjs.com.cn/
1. node/express MDN 教程：https://developer.mozilla.org/zh-CN/docs/learn/Server-side/Express_Nodejs

# 8. 后端进阶：数据持久化，用户系统，Cookie，密码加密

## 任务

改进上节任务中的 vue2.x/express 版本的 TodoMVC，做到：

1. 后端不再使用内存保存数据，改用文件保存，以免在 http 服务重启后丢失数据；
1. 自行设计前端用户注册、登入、登出页面，以及相关后端功能，把不同用户的数据保存在后端的不同文件内，用户应能够读写各自的数据；
1. 用户使用密码字符串进行注册、登录，后端不应保存密码明文（携程等大厂都犯过这个错），应加密之后保存。

- 着重体会 “前端页面 <-- HTTP API --> 后端 HTTP 服务 <--> 数据持久层(后端文件/数据库)” 这个 web 开发常见架构

## 推荐教程和参考文档

1. NodeJS 文件读写 API: http://nodejs.cn/api/fs.html
2. HTTP Cookie: https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Cookies
3. Express 读 Cookie: https://www.expressjs.com.cn/resources/middleware/cookie-parser.html
4. Express 写 Cookie: https://www.expressjs.com.cn/4x/api.html#res.cookie
5. 密码加密可用这个库: https://preview.npmjs.com/package/bcryptjs

# 9. TypeScript: 为大中型全栈项目做准备

## 任务

用 Typescript 改写 react/express 版本 TodoMVC 前后端，要求不能存在任何 `any` 类型

## 推荐教程和参考文档

1. 以 TodoMVC 为例入门 TS https://ts.chibicode.com/todo/
1. 泛型入门 https://ts.chibicode.com/generics/
1. TS 入门教程 https://github.com/xcatliu/typescript-tutorial
1. TS 教程 https://willh.gitbook.io/typescript-tutorial/
1. TS 非官方中文站 https://zhongsp.gitbooks.io/typescript-handbook/content/

注意事项：

- 先不需要深究 TS 里面那些高级功能，如 infer 等。我们不是框架作者，只是使用者，学会用 TS 做基本类型标注即可。结合 VSCode, TS, React hooks, Vue 3 Compostion API, JSX(TSX), 可以获得极好的开发体验，有效降低开发心智负担

<strike># 10. Web 全栈前沿技术：Blitz.js 全栈框架 + Prisma 数据访问层 + 前端 Chakra UI 样式与组件库

## 任务

用 Blitz.js 全栈框架复刻功能更复杂的 Microsoft To-Do （https://to-do.live.com/）：

1. 先仔细研究 Microsoft To-Do 功能，确定前后端数据结构
1. 使用 Prisma schema 描述后端数据结构
1. 在 blitz 中构造前端 react 组件树，以及后端 query/mutation，复刻完整的 To-Do 功能
1. 提供适当的 HTTP 缓存和 CORS 支持，并提高 HTTP Headers 安全性
1. 组件样式可考虑使用 Chakra UI

- 之前 TodoMVC 后端数据结构简单，我们使用内存、文件等形式来保存。微软 To-Do 数据结构较复杂，这次我们需要使用数据库来保存。但鉴于 SQL、MongoDB 等后端常用数据库技术超出了本次教学范围，我们这次使用 prisma 数据访问层来包装后端 SQL 数据库，隐藏起了 SQL 的技术细节，以便让大家更加集中精力学习 Web 前后端相关内容；
- 请着重体会 Blitz 框架前后端贯通的 “无 HTTP API” 写法，前后端 API 的函数签名、Typescript 类型都自动推导，非常适合快速开发。

## 推荐教程和参考文档

1. Blitz 官网: https://blitzjs.com/
1. Blitz 文档中文版: https://github.com/blitz-js/zh-hans.blitzjs.com (正在翻译中)
1. Prisma 官网：https://www.prisma.io/
1. HTTP: https://developer.mozilla.org/zh-CN/docs/Web/HTTP
1. Chakra UI: https://chakra-ui.com/  
   </strike>
