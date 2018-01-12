# 关于 Kanboard 的中文介绍

具体的内容请查看[官网](https://kanboard.org/)

**Kanboard 是一个免费和开源的 Kanban 项目管理工具**

![Kanban](https://kanboard.org/assets/img/board.png)

它的长处在以下这些:

- 可视化你的工作
- 规划你进行中的工作,**让你可以集中在你的目标**
- 在项目面板上通过简单的拖拽就可以实现任务的控制
- 可以自己部署
- 超级简单的安装

---

* [功能](README_CN.md#功能)
* [插件](README_CN.md#插件)
* [下载最新版本]()
* [文档]

    * [需求]()
    
    * [安装向导]()
    
    * [更新到新版本]()
    
    * [Docker 镜像用法]()    
    
* [论坛]()
* [提交 Bug]()
* [Rss 订阅]()
* [Twitter]()

## 功能
---
### 极简主义
> 没有花俏的用户界面, Kanboard 将所有精力用于将功能简单化和最小化. Kanboard 本身提供的功能都是有限的(译者注,这其实是优点,如果需要更多的功能可以使用插件来完成).

### 任务简单,清晰,可视
> Kanban 面板是最简单的查看当前项目进度的方式,因为这一切都是可视的,无需培训,无需更多的介绍,所有人都可以通过 Kanban 知道自己的任务和当前项目的进度.

### 在不同的Kanban 列(译者注,别的项目有的称为管道- Pipeline)可以任意的拖拽
> ![Drag Drop](https://kanboard.org/assets/img/drag-and-drop.png)

> 你可以随时增加或删除Kanban 列来适应你自己的项目

### 限制同时开工任务,让任务执行更有效
> ![](https://kanboard.org/assets/img/task-limit.png)

> 避免同时进行多个任务(multitask),更加专注于当前的任务.如果超过设定的限制的话,这一列(Column)会高亮显示.

### 搜索和过滤任务
> ![](https://kanboard.org/assets/img/search.png)
> Kanboard 提供了一个简单的查询语言(Query Language),可以随时查询任务的情况.通过在面板中增加不同的搜索条件,可以实现很好的动态查询的效果.可以通过任务指派人(assignee),描述(description),分类(category),截止日期(due date)等等.

### 任务,子任务,附件和评论
> * 通过将任务分解成子任务,可以更好的估算完成时间和复杂度
> * 也可以使用 Markdown 格式来进行任务的描述.
> * 可以为任务添加附件,添加评论,修改颜色,修改分类,修改任务指派人,修改截止日期
> * 可以在不同的项目间,移动和复制任务.

### 自动化操作
> ![](https://kanboard.org/assets/img/automatic-actions.png)
> 不再重复发明轮子,可以通过自动化的动作让流程更加智能,不用再同样的事情上一次又一次的执行.可以自动的修改任务指派人,颜色,分类,几乎所有的所有.

### 30+的语言支持
> 感谢来自于不同国家的广泛的爱好者的付出. Kanboard 已经被翻译成了 Bahasa Indonesia, Bosnian, Brazilian Portuguese, Chinese, Chinese (Taiwan), Czech, Danish, Dutch, English, Finnish, French, German, Greek, Hungarian, Italian, Japanese, Korean, Malay, Norwegian, Polish, Portuguese, Romanian, Russian, Serbian, Spanish, Swedish, Thai, Turkish, Vietnamese.

### 多种验证方式的支持
> Kanboard 可以链接到你的 LDAP/Active Directory或者使用 OAuth2提供商(Google,GitHub,GitLab, 等等)

### 免费和开源的软件
> Kanboard 是以** MIT** 协议发布的,软件主要有Frédéric Guillot来维护和开发,但是有操作190个其他的贡献者.

---
## 插件

你可以通过安装下面的扩展来增加Kanboard的特性

### [移动卡片到指定的列( Column) 里时自动分配分类](https://github.com/dmorlitz/kanboard-TaskAssignCategory)
> 增加一个自动的动作,允许你设置一个移动到指定的列的时候自动设置的分组.
> By David Morlitz

### [为未指派日期的卡片设置时间](https://github.com/dmorlitz/kanboard-TaskAssignDateToUndated)
> 增加一个自动的动作,为未支配日期的卡片自动设置一个到期日期,帮助在导出 ICS 的时候可以更好的显示在日历中.
> By David Morlitz

### [自动邮件相关扩展动作](https://github.com/creecros/SendEmailCreator)
> 这个插件为 Kanboard 增加了一下的3个新的自动动作
> - 给任务指派人发送 Email
> - 给任务创建者发送 Email
> - 根据截至日期发送 Email
> By Craig Crosby

### [自动创建子任务动作](https://github.com/creecros/AutoSubtasks)
> 当一个任务被创建或者在不同的列间移动的时候,自动创建子任务
> By Craig Crosby

### [广播](https://github.com/kanboard/plugin-broadcast)
> 通过系统内部或者 Email 进行消息广播的插件
> By Frédéric Guillot

### [Beanstalk](https://github.com/kanboard/plugin-beanstalk)
> 使用 Beanstalk 进行后台任务的执行
> By Frédéric Guillot

### [聊天](https://github.com/kanboard/plugin-chat)
> 为小规模团队提供的聊天小程序
> By Frédéric Guillot

### [Amazon S3存储](https://github.com/kanboard/plugin-s3)
> 该插件可以允许你将上传的附件保存在 AmazonS3上,而不是保存在本地.
> By Frédéric Guillot

### [Bitbucket Webhook](https://github.com/kanboard/plugin-bitbucket-webhook)
> 绑定 Bitbucket 的 webhook 到 Kanboard 的自动化动作上.
> By Frédéric Guillot

### [预算-Budget](https://github.com/kanboard/plugin-budget)
> 预算计划,通过对子任务的时间跟踪实现:创建预算基线,查看根据子任务的时间的跟踪来计算费用,管理每个用户的单位时费率.
> By Frédéric Guillot

### [日历](https://github.com/kanboard/plugin-calendar)
> 在 Kanboard 中集成日历功能
> By Frédéric Guillot

### [客户端SSL 验证授权](https://github.com/kanboard/plugin-client-certificate)
> 使用 SSL 客户端验证
> By Frédéric Guillot

### [封面图(Coverimage)](https://github.com/BlueTeck/kanboard_plugin_coverimage)
> 插件为Board 增加封面图的功能
> By Frédéric Guillot

### [数据库存储](https://github.com/kanboard/plugin-database-storage)
> 该插件可以将用户上传的文件保存在数据库中.
> By Frédéric Guillot

### [截止日期排序](https://github.com/dmorlitz/kanboard-duedate)
> 支持面板中通过卡片的截止日期进行排序
> By David Morlitz

### [甘特图](https://github.com/kanboard/plugin-gantt)
> 项目和任务的甘特图展现
> By Frédéric Guillot

### [GitHub 验证](https://github.com/kanboard/plugin-github-auth)
> 使用 GitHub 作为验证提供方
> By Frédéric Guillot

### [用作 GitHub 前台](https://github.com/kanboard/plugin-github-frontend)
> 使用 Kanboard 来管理 GitHub Issues
> By Frédéric Guillot

### [GitHub Webhook](https://github.com/kanboard/plugin-github-webhook)
> 链接 Github Webhook 到 Kanboard 的自动任务
> By Frédéric Guillot

### [GitLab 验证](https://github.com/kanboard/plugin-gitlab-auth)
> 使用 GitLab 作为验证提供商
> By Frédéric Guillot

### [GitLab Webhook](https://github.com/kanboard/plugin-gitlab-webhook)
> 链接 GitLab webhook 到 Kanboard 的自动任务
> By Frédéric Guillot

### [Gravatar(头像)](https://github.com/kanboard/plugin-gravatar)
> 使用 Gravatar 来显示用户头像.
> By Frédéric Guillot

### [Gogs Webhook](https://github.com/kanboard/plugin-gogs-webhook)
> 链接 Gogs webhook 到 Kanboard 的自动任务
> By Frédéric Guillot

### [Google 验证](https://github.com/kanboard/plugin-google-auth)
> 使用 Google 作为验证提供商
> By Frédéric Guillot

### [Hipchat](https://github.com/kanboard/plugin-hipchat)
> 在 Hipchat 中收到个人或者项目的通知
> By Frédéric Guillot

### [Jabber](https://github.com/kanboard/plugin-jabber)
> Jabber 中收到个人或者项目的通知
> By Frédéric Guillot

### [Mailgun](https://github.com/kanboard/plugin-mailgun)
> 使用 MailgunAPI 发送邮件和通过邮件创建任务
> By Frédéric Guillot

### [Mattermost](https://github.com/kanboard/plugin-mattermost)
> 发送 Kanboard 的通知到 Mattermost
> By Frédéric Guillot

### [Metadata 管理器](https://github.com/BlueTeck/kanboard_plugin_metadata)
> 这个插件安装后,提供了一个 GUI(用户界面),可以单独设置任务,项目和用户的 metadata(元数据信息)
> By BlueTeck

### [Milestone(里程碑)](https://github.com/oliviermaridat/kanboard-milestone-plugin)
> 可以通过一个里程碑来查看关联的任务
> By Olivier Maridat

### [截止日期到后,将任务移动到指定的列](https://github.com/dmorlitz/kanboard-TaskMoveOnDueDate)
> 增加一个自动的动作,可以在任务的截止日期到达后将卡片移动到指定的列
> By David Morlitz

### [OAuth2](https://github.com/kanboard/plugin-oauth2)
> 通用的 OAuth2插件
> By Frédéric Guillot

### [覆盖翻译](https://github.com/BlueTeck/kanboard_plugin_overwrite_translation)
> 覆盖默认的翻译,而不用接触到 Kanboard 的文件
> By BlueTeck

### [Postmark](https://github.com/kanboard/plugin-postmark)
> 使用 PostmarkAPI 来发送邮件和通过邮件来创建任务
> By Frédéric Guillot

### [Push out due date on cards when moving to specific columns](https://github.com/dmorlitz/kanboard-TaskPushDate)
> Adds an automatic action which allows you to push the due date a specified number of days when moving cards to a specific column.
> By David Morlitz

### [RabbitMQ](https://github.com/kanboard/plugin-rabbitmq)
> 使用 RabbitMQ 作为后台任务处理
> By Frédéric Guillot

### [关系图](https://github.com/xavividal/kanboard-plugin-relationgraph)
> 使用图形库技术来显示任务间的关系
> By Xavier Vidal

### [使用 LDAP 用户提供商实现反向代理身份验证](https://github.com/kanboard/plugin-reverse-proxy-ldap)
> 使用反向代理方法验证用户身份，通过LDAP目录填充用户信息。
> By Frédéric Guillot

### [RocketChat](https://github.com/kanboard/plugin-rocketchat)
> RocketChat 中接受个人或项目通知
> By Frédéric Guillot

### [自行注册](https://github.com/kanboard/plugin-registration)
> 该插件可以允许用户在 Kanboard 系统上自己注册
> By Frédéric Guillot

### [Sendgrid](https://github.com/kanboard/plugin-sendgrid)
> 使用 Sendgrid API 来发送 Email 并通过 Email 创建任务
> By Frédéric Guillot

### [Slack](https://github.com/kanboard/plugin-slack)
> 通过 Slack 来接受个人或项目通知
> By Frédéric Guillot

### [SMS 2步认证](https://github.com/kanboard/plugin-sms-2fa)
> 使用 SMS 文本消息实现2步认证
> By Frédéric Guillot

### [子任务广播](https://github.com/kanboard/plugin-subtask-forecast)
> 此插件显示用户日历中子任务的估计值。必须填写用户时间表才能查看日历中的时间段。
> By Frédéric Guillot

### [子任务截止日期](https://github.com/eSkiSo/Subtaskdate)
> 该插件为子任务增加一个截止日期
> By Manuel Raposo

### [任务面板日期](https://github.com/kanboard/plugin-task-board-date)
> 为任务添加新的日期字段以定义面板和仪表板上的可视性。
> By Frédéric Guillot

### [时间表](https://github.com/kanboard/plugin-timetable)
> 为用户提供工作时间表管理。
> By Frédéric Guillot

### [时间跟踪编辑器](https://github.com/stinnux/kanboard-Timetrackingeditor)
> 手动添加和编辑时间跟踪条目，添加评论和选择收费/不收费时间跟踪条目。导出时间跟踪条目为html。
> By Stinnux

### [时间间隔按钮](https://github.com/mrozigor/kanboard-add-time-interval-plugin)
> 简单的插件添加按钮，以增量更改任务花费的时间。
> By Igor Mroz

### [Wunderlist](https://github.com/EpocDotFr/kanboard-wunderlist)
> 这个插件允许你通过上传一个wunderlist导出文件直接从kanboard的用户界面导入wunderlist任务和列表。
> By Maxime (Epoc)

### [评论工具提示](https://github.com/enricofrigo/kanboard/tree/master/plugin-comment-tooltip)
> 显示任务的评论作为工具提示像在较旧的kanboard版本中一样。
> By Enrico Frigo

### [Telegram](https://github.com/manuvarkey/kanboard-plugin-telegram)
> 在 Telegram 中收到个人或项目通知
> By Manu Varkey


