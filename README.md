![2233](docs/imgs/2233.png)

<div align="center">

<h1 align="center">

BiliBiliTool

</h1>

[![GitHub Stars](https://img.shields.io/github/stars/RayWangQvQ/BiliBiliToolPro?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/RayWangQvQ/BiliBiliToolPro?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/network)
[![GitHub Issues](https://img.shields.io/github/issues/RayWangQvQ/BiliBiliToolPro?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/issues)
[![GitHub Contributors](https://img.shields.io/github/contributors/RayWangQvQ/BiliBiliToolPro?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/graphs/contributors)
[![GitHub All Releases](https://img.shields.io/github/downloads/RayWangQvQ/BiliBiliToolPro/total?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/releases)
![GitHub Release (latest SemVer)](https://img.shields.io/github/v/release/RayWangQvQ/BiliBiliToolPro?style=flat-square)
[![GitHub License](https://img.shields.io/github/license/RayWangQvQ/BiliBiliToolPro?style=flat-square)](https://github.com/RayWangQvQ/BiliBiliToolPro/blob/main/LICENSE)

</div>

**BiliBiliTool 是一个自动执行任务的工具，当我们忘记做某项任务时，它会像一个贴心小助手，按照我们预先吩咐它的命令，在指定频率、时间范围内帮助我们完成计划的任务。**

详细功能如下：

- **每日获取满额升级经验（登录、投币、点赞、分享视频）（支持指定支持up主）**
- **每天漫画签到**
- **每天直播签到**
- **直播中心银瓜子兑换为硬币**
- **每月领取大会员赠送的 5 张 B 币券和福利（忘记或者不领就浪费了哦）**
- **每月领取大会员漫画福利**
- **月底在 B 币券过期前进行充电（支持指定想要支持的up主，如果没有喜欢的up，也可以为自己充个电啊，做个用爱为自己发电的人~）**
- **直播中心天选时刻自动参与抽奖**
- **批量取关**
- **大会员大积分任务**
- **支持多账号**
- **理论上支持所有远端的日志推送（默认支持推送到Telegram、企业微信、钉钉、PushPlus、Server酱、钉钉、酷推，另外也支持自定义推送到任意api）**
---
[目录]

<!-- TOC depthFrom:2 -->

- [1. 如何使用](#1-如何使用)
    - [1.1. 部署 BiliBiliTool](#11-部署-bilibilitool)
        - [1.1.1. 方式一：青龙（推荐）](#111-方式一青龙推荐)
        - [1.1.2. 方式二：Docker或Podman容器化运行](#112-方式二docker或podman容器化运行)
        - [1.1.3. 方式三：下载程序包到本地或服务器运行](#113-方式三下载程序包到本地或服务器运行)
        - [1.1.4. 方式四：腾讯云函数SCF](#114-方式四腾讯云函数scf)
        - [1.1.5. 方式五：~~GitHub Actions~~](#115-方式五github-actions)
        - [1.1.6. 方式六：Chart部署](#116-方式六chart部署)
    - [1.2. 消息推送（可选）](#12-消息推送可选)
- [2. 功能任务说明](#2-功能任务说明)
- [3. 个性化自定义配置](#3-个性化自定义配置)
- [4. 多账号支持](#4-多账号支持)
- [5. 常见问题](#5-常见问题)
- [6. 版本发布及更新](#6-版本发布及更新)
- [7. 成为开源贡献成员](#7-成为开源贡献成员)
    - [7.1. 贡献代码](#71-贡献代码)
    - [7.2. 贡献文档](#72-贡献文档)
- [8. 捐赠支持](#8-捐赠支持)
- [9. 其他](#9-其他)

<!-- /TOC -->

---
**Github 仓库地址：[RayWangQvQ/BiliBiliToolPro](https://github.com/RayWangQvQ/BiliBiliToolPro)**

**注意：**

- **本应用仅用于学习和测试，作者本人并不对其负责，请于运行测试完成后自行删除，请勿滥用！**
- **所有代码都是开源且透明的，任何人均可查看，程序不会保存或滥用任何用户的个人信息**
- **应用内几乎所有功能都开放为了配置（如任务开关、日期、id等），详细信息可阅读配置文档，请自己对配置负责**

本地运行图示：

![运行图示](docs/imgs/run-exe.png)

_（如果图片挂了，请自己架梯子，没有的也可以先参考 [我的博客](https://www.cnblogs.com/RayWang/p/13909784.html)，但内容不保证最新)_


## 1. 如何使用

BiliBiliTool 实现自动完成任务的原理，是通过调用一系列开放的api实现的。

**要使用 BiliBiliTool，很简单，按照下面教程部署完成，运行后扫码登录即可。**

### 1.1. 部署 BiliBiliTool

支持多种部署方式，以下选择任一适合自己的方式即可。

#### 1.1.1. 方式一：青龙（推荐）

[>>青龙部署教程](qinglong/README.md)

#### 1.1.2. 方式二：Docker或Podman容器化运行

[>>Docker部署说明](docker/README.md)

[>>Podman部署说明](podman/README.md)

#### 1.1.3. 方式三：下载程序包到本地或服务器运行

[>>本地部署说明](docs/runInLocal.md)

#### 1.1.4. 方式四：腾讯云函数SCF

当前腾讯云函数已改为收费模式，不推荐。

[>>腾讯云函数部署说明](tencentScf/README.md)


#### 1.1.5. 方式五：~~GitHub Actions~~

暂时删掉该方式避避风头。

**建议所有使用该方式运行的朋友，暂时先替换其他运行方式，避免造成不必要的损失。**

#### 1.1.6. 方式六：Chart部署

[>>Chart部署说明](helm/README.md)

### 1.2. 消息推送（可选）

如果配置了推送，执行成功后，指定的接收端会收到推送消息，推送效果如下所示：

![微信推送图示](docs/imgs/wechat-push.png)

目前默认支持**PushPlus推送、企业微信应用推送、企业微信推送、钉钉推送、Microsoft Teams推送、Telegram推送、Server酱推送和酷推QQ推送**（以上顺序即为个人推荐的排序），如果需要推送到其他端，也可以配置为任意的可以接受消息的Api地址，关于如何配置推送请详见下面的**个性化自定义配置**章节。

## 2. 功能任务说明
这里的**任务**是指一组功能的集合，是工具每次运行的最小单位。工具启动后会根据我们输入的任务编码，运行相应的任务，如：

```
dotnet Ray.BiliBiliTool.Console.dll --runTasks=Daily
```

程序启动后，会执行任务Code为 `Daily` 的`每日经验任务`。

可以通过使用 `&` 符拼接多个任务，程序启动后会按顺序依次执行指定的任务集合，如

```
dotnet Ray.BiliBiliTool.Console.dll --runTasks=Daily&LiveLottery
```

会依次运行`每日任务`和`天选抽奖任务`。

一般来说，每个任务都有一个 GitHub Actions 的工作流脚本（workflow）对应，划分的依据主要是根据功能需求，其次是触发频率（比如，有些每天只需运行一次，有些需要允许多次）。

任务列表如下：

| 任务名 | Code | 功能 | 默认WorkFlow文件 | GithHub Environments | 推荐运行频率 | 备注 |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: |
| 每日任务 | Daily | 完成每日任务获取满额65点经验（登录、观看视频、分享视频、投币），以及签到、领福利和充电等附属功能 | bilibili-daily-task.yml | Production | 每天一次 | |
| 天选时刻抽奖 | LiveLottery | 直播中心天选时刻抽奖 | live-lottery-task.yml | LiveLottery | 建议每天运行0-4次内 | 对应Actions工作流默认是关闭的，需要添加key为`ISOPENLIVELOTTERYTASK`、值为`true`的secret来手动开启；大部分抽奖都需要关注主播，介意的不要开启 |
| 批量取关 | UnfollowBatched | 批量取关指定分组下的所有关注（主要用于清理天选抽奖而产生的关注） | unfollow-batched-task.yml | 无 | 需要时手动运行 | 需要通过配置指定2个参数：`GroupName`（分组名称，如`天选时刻`）和`Count`（目标取关个数，-1表示全部），应用会倒序从后往前取关指定个数 |
| 大会员大积分 | VipBigPoint | 大会员大积分任务（签到、浏览、观看） | 无 | 无 | 每天凌晨一点运行 | |
| 测试Cookie | Test | 测试Cookie是否正常 | 无，可以使用empty-task.yml来运行 | 无 | 需要时手动运行 | 主要用于调试 |
| 空模板 | 无（只用于 GitHub Actions ） | 用于 GitHub Actions 运行指定的任意任务 | empty-task.yml | 无 | 需要时手动运行 | 需要通过配置指定要运行的任务Code（多个使用英文逗号分隔），主要用于调试 |

## 3. 个性化自定义配置

[>>点击查看配置说明文档](docs/configuration.md)

## 4. 多账号支持

~~对于 GitHub Actions 托管的，可以通过添加 Key 为 `COOKIESTR2` 和 `COOKIESTR3` 的 Secret ，来支持最多 3 个账号。~~

Docker或其他方式托管的，因配置项 `BiliBiliCookies` 被设计为一个字符串数组，所以理论可以添加任意个数的账号，例：
```
 "BiliBiliCookies": [
    "cookies1",
    "cookies2",
    "..."
  ],

```

使用环境变量配置的话，可以添加 Key 为 `Ray_BiliBiliCookies__2`、`Ray_BiliBiliCookies__3`、`Ray_BiliBiliCookies__4`...的环境变量，以此类推。

## 5. 常见问题

[>>点击查看常见问题文档](docs/questions.md)

[Issues（议题）](https://github.com/RayWangQvQ/BiliBiliToolPro/issues)板块可以用来提交**Bug**和**建议**；

[Discussions（讨论）](https://github.com/RayWangQvQ/BiliBiliToolPro/discussions)板块可以用来**提问**和**讨论**。

大部分问题其实都可以在文档、议题和讨论中找到答案。

所以如果你有疑问，

* 请先确认是否可以通过升级到最新版本解决
* 然后搜索文档（特别是配置说明文档和常见问题文档）、议题和讨论，查看是否已有其他人遇到相同问题、是否已有解决方案

如果确认还未解决，可以自己提交 Issue，或发布 Discussions 与大家一起探讨，我会尽快确认并解决。

（关于如何正确的提交Issue，请详见**常见问题文档**）。

## 6. 版本发布及更新

当前正处于稳定的迭代开发中，~~正常情况下每 2 周会发布一个小版本~~，详细待更新和计划内容可参见 [Projects](https://github.com/RayWangQvQ/BiliBiliToolPro/projects) 和 [Issues](https://github.com/RayWangQvQ/BiliBiliTool/issues) 。

关于新版本发布后，如何同步最新的内容到自己 Fork 的仓库，可参考**常见问题文档**中的 《**我 Fork 之后如何同步原作者的更新内容？**》章节。

建议每个人都开启自动同步更新，因为越新的版本功能越完善、对账号来说也越安全。

也建议把右上角的 Star 点一下，这样有重要更新时就会有邮件推送了。

## 7. 成为开源贡献成员

### 7.1. 贡献代码
如果你有好的想法，欢迎向仓库贡献你的代码，贡献步骤：

* 搜索查看 Issue，确定是否已有人提过同类问题

* 确认没有同类 Issue 后，自己可新建 Issue，描述问题或建议

* 如果想自己解决，请 Fork 仓库后，在**develop 分支**进行编码开发，完成后**提交 PR 到 develop 分支**，并标注解决的 Issue 编号

我会尽快进行代码审核，测试成功后会合并入 main 主分支，提前感谢您的贡献。

### 7.2. 贡献文档
文档部分由于我个人精力有限（写文档比写代码累多了），所以有些地方写的很简略，甚至有遗漏和错别字，不能贡献代码的朋友也欢迎来一起维护文档，欢迎 PR 来纠正我，一样都算是对开源做贡献了。

## 8. 捐赠支持

[>>捐赠留言及回复](docs/donate-list.md)

个人维护开源不易

如果觉得我写的程序对你小有帮助

或者，就是单纯的想集资给我买瓶霸王增发液

那么下面的赞赏码可以扫一扫啦

（赞赏时记得留下【昵称】和【留言】~ 另外我发现很多留言想要进群或者加好友的，一定一定要记得留下微信号哈，微信赞赏页面是看不到微信号的）

**☟☟☟ 扫码自动赞赏 1 元：☟☟☟**

![赞赏码](docs/imgs/donate.jpg)

> 项目中的优先支持的UP主的配置项，默认是作者的 UpId （只是作为了 JSON 配置文件的默认值，代码是干净的），需要更改的话，直接修改相应配置即可（secrets或环境变量等各种方式都行）。

当然，不改的话，也算是另一种捐赠支持作者的方式啦。

感谢支持~

## 9. 其他

`API`参考：

- [www.bilibili.com](https://www.bilibili.com/)

- [SocialSisterYi/bilibili-API-collect](https://github.com/SocialSisterYi/bilibili-API-collect)

- [JunzhouLiu/BILIBILI-HELPER](https://github.com/JunzhouLiu/BILIBILI-HELPER)

感谢`JetBrain`提供的免费证书支持：

Thanks to `JetBrain` for the free certificate support:

![ReSharper logo](https://resources.jetbrains.com/storage/products/company/brand/logos/ReSharper.svg)

