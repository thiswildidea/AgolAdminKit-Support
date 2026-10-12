---
title: Privacy Policy
---

# Privacy Policy — Portal One For ArcGIS

**Effective 12 October 2026.** Portal One For ArcGIS was previously called AGOL-Enterprise
Admin Kit; this policy covers it under either name. The versions before it, effective 24
September and 10 October 2026, left out Microsoft Store, which the application asks about
updates and about its optional subscription; the first of them also said it talks to your
portal alone and never writes a password to disk, when it also talks to map services and to
this website and keeps a password when you ask it to — all as described below.

## The short version

This application collects nothing. It has no analytics, no telemetry, and no
crash reporting service. Nothing about you, your organization, or your use of
the application is sent to the developer or to any third party — not on first
run, not on failure, not ever.

The application talks to the ArcGIS Online or ArcGIS Enterprise portals whose
addresses **you** enter, to the map services, basemaps and elevation data their
content points at, to this website, from which its Help page reads the help, and
to Microsoft Store, about updates and the optional subscription. Everything it
produces stays on your computer.

## What the application stores, and where

All of it lives in the application's own folder on your computer, under
`%LOCALAPPDATA%\Packages\`. None of it is uploaded anywhere.

| File | What it holds |
| --- | --- |
| `tokens.dat` | Sign-in tokens for the portals you connect to, and the password of a connection you signed in to with a username and password and asked to stay signed in |
| `portals.json` | The portal addresses and display names you have added |
| `offboarding-journal.json` | A record of transfers and deletions you performed, so they can be reviewed and undone |
| `acknowledged-findings.json` | Which audit findings you have marked as reviewed |
| `activation.log` | When the application was started, and counts of items scanned |
| `crash.log` | Written only if the application fails unexpectedly |

### About your credentials

Sign-in tokens are encrypted with the Windows Data Protection API, scoped to
your Windows user account. They cannot be read by another user on the same
computer, and they do not survive being copied to another machine. If you sign
in through the browser window, Microsoft Edge WebView2 keeps its own session
data in the same application folder.

Your password is written to disk in one case only: you signed in with a username
and password and chose to stay signed in. That way of signing in issues no token
that can renew itself, so the password is kept instead — encrypted in `tokens.dat`
the same way as the tokens, and sent only to the portal it belongs to. Signing in
through the portal's own page, or without staying signed in, keeps no password.

### About the logs

`activation.log` and `crash.log` record names, counts and error types — for
example "member list read, members=5". They do not record passwords, tokens, or
the contents of your data. They are never transmitted. You can delete them at
any time.

## What the application sends, and to whom

**To your portal**, only the requests needed to do what you asked: listing
content, reading item details, transferring ownership, deleting an item you
selected. Those requests carry your access token in an authorization header so
the portal knows who is asking. The application will also contact
`www.arcgis.com` when you connect to ArcGIS Online, because that is where ArcGIS
Online lives.

**To map services**, when you open something in the map or scene viewer: the
basemaps your portal offers (on ArcGIS Online, and on many ArcGIS Enterprise
portals, Esri's basemap services), Esri's world elevation for scenes on ArcGIS
Online, and the services the layers you open point at, which may be another
organization's servers. Your sign-in goes only to your portal and to services
that are part of it — on ArcGIS Online, Esri's own services such as routing,
which bill your organization's credits. A layer on another organization's server
is requested without it.

**To this website**, when you open the Help page: the help in the application's
language, and its screenshots, are downloaded from `thiswildidea.github.io`,
served by GitHub Pages, so that the help is current. The request names the
language it asks for and, like any request on the internet, comes from your
network address; it carries no token, no account, and nothing about your
organization. GitHub's privacy statement covers what GitHub Pages records. When
the website cannot be reached, the help installed with the application is shown
instead.

**To Microsoft Store**, through Windows' own Store services: whether a newer
version of the application is available, and — for the optional monthly
subscription that takes the "Not subscribed" mark off its pages — what the
subscription costs and whether your Microsoft account holds it. Buying,
renewing and cancelling it happen in Microsoft Store's own windows, and payment
is handled by Microsoft under Microsoft's privacy statement. The application
sends nothing of yours with these requests — no portal, no token, no content —
and keeps no record of a purchase: it asks the Store again each time it starts.

There is no other network destination, and there is no developer server:
nothing the application sends reaches the developer.

## What the developer can see

Nothing from the application. There is no account, no registration, and no
server to collect anything. If you subscribe, Microsoft gives the developer the
sales and acquisition reports it gives every publisher in its Store, which do not
identify you. If you write to the support address below, the developer sees only
what you choose to put in that email.

## Children

The application is a professional administration tool and is not directed at
children. It collects no information from anyone, including children.

## Changes

If this policy changes, the revised version will be published at this address
with a new effective date.

## Contact

Questions about this policy, or about anything the application does with your
data: **gaqo@outlook.com**

When reporting a problem, please do not attach passwords, tokens, or files from
the application's storage folder.

---

# 隐私政策 — Portal One For ArcGIS

**生效日期：2026 年 10 月 12 日**。Portal One For ArcGIS 原名 AGOL-Enterprise Admin Kit，本政策对两个名称同样适用。之前的两版（2026 年 9 月 24 日和 10 月 10 日生效）都漏写了 Microsoft Store——应用会向它查询更新和可选的订阅；其中 9 月 24 日那版还写着应用只与你的门户通信、从不把密码写入磁盘，而实际上它还会访问地图服务和本网站，并会在你要求时保存密码。详见下文。

## 一句话版本

本应用**不收集任何数据**。没有分析统计，没有遥测，没有崩溃上报服务。关于你、你的组织、你如何使用本应用的任何信息，都不会发送给开发者或任何第三方——首次运行时不会，出错时不会，任何时候都不会。

本应用与以下服务器通信：**你自己填写地址**的 ArcGIS Online 或 ArcGIS Enterprise 门户，门户内容所指向的地图服务、底图和高程数据，本网站（应用的“帮助”页面从这里读取帮助），以及 Microsoft Store（查询更新和可选的订阅）。它产生的一切都留在你自己的电脑上。

## 本应用保存什么，保存在哪

全部位于本机 `%LOCALAPPDATA%\Packages\` 下应用自己的文件夹内，不会上传到任何地方。

| 文件 | 内容 |
| --- | --- |
| `tokens.dat` | 你所连接门户的登录令牌；以及你用用户名和密码登录并选择保持登录的连接的密码 |
| `portals.json` | 你添加的门户地址与显示名称 |
| `offboarding-journal.json` | 你执行过的转移与删除记录，用于复查和撤销 |
| `acknowledged-findings.json` | 你已标记为"已查看"的审计发现项 |
| `activation.log` | 应用的启动时间，以及扫描到的条目数量 |
| `crash.log` | 仅在应用意外失败时写入 |

### 关于你的凭据

登录令牌使用 Windows 数据保护 API 加密，作用域绑定到你的 Windows 用户账号。同一台电脑上的其他用户无法读取，复制到另一台机器也无法解密。如果你通过浏览器窗口登录，Microsoft Edge WebView2 会在同一个应用文件夹内保存它自己的会话数据。

**只有一种情况会把密码写入磁盘**：你用用户名和密码登录，并选择了保持登录。这种登录方式不会签发可以自行续期的令牌，所以应用改为保存密码——与令牌一样加密保存在 `tokens.dat` 中，并且只发送给它所属的门户。通过门户自己的登录页面登录，或不选择保持登录，都不会保存密码。

### 关于日志

`activation.log` 和 `crash.log` 只记录名称、数量和错误类型——例如"成员列表已读取，成员数=5"。它们**不记录**密码、令牌或你的数据内容，也从不传输。你可以随时删除它们。

## 本应用向谁发送什么

**发给你的门户**的，只有完成你所要求的操作所必需的请求：列出内容、读取条目详情、转移归属、删除你选中的条目。这些请求在授权头中携带你的访问令牌，以便门户识别请求者身份。当你连接 ArcGIS Online 时，应用还会访问 `www.arcgis.com`，因为那就是 ArcGIS Online 所在之处。

**发给地图服务**的，是你在地图查看器或场景查看器中打开内容时所需的请求：门户提供的底图（在 ArcGIS Online 上，以及许多 ArcGIS Enterprise 门户上，是 Esri 的底图服务）、ArcGIS Online 上场景所用的 Esri 全球高程，以及你打开的图层所指向的服务——它们可能位于其他组织的服务器上。你的登录凭据只发送给你的门户及其自身的服务（在 ArcGIS Online 上，包括路径分析等会消耗组织积分的 Esri 服务）；其他组织服务器上的图层，请求时不带凭据。

**发给本网站**的，是你打开“帮助”页面时的请求：应用从 `thiswildidea.github.io`（由 GitHub Pages 提供）下载应用界面语言的帮助及其截图，让帮助保持最新。请求中只包含所需帮助的语言，并且和互联网上的任何请求一样，来自你的网络地址；它不带令牌、不带账号，也不含任何关于你组织的信息。GitHub Pages 会记录什么，由 GitHub 的隐私声明说明。无法访问本网站时，改为显示随应用安装的帮助。

**发给 Microsoft Store**的，经由 Windows 自带的应用商店服务：是否有新版本可以更新；以及可选的按月订阅（用于去掉页面上的“未订阅”标记）的价格、你的 Microsoft 账户是否已经订阅。购买、续订和取消都在 Microsoft Store 自己的窗口中进行，付款由 Microsoft 依据其隐私声明处理。这些请求不携带你的任何信息——没有门户、没有令牌、没有内容——应用也不保存购买记录，每次启动时重新向应用商店询问。

除此之外没有任何其他网络目的地，**也不存在开发者服务器**：应用发出的任何内容都不会到达开发者手中。

## 开发者能看到什么

应用不会让开发者看到任何东西。本应用没有账号体系、无需注册，也不存在任何用于收集信息的服务器。如果你订阅，Microsoft 会向开发者提供它给每个商店发布者的销售和获取报告，这些报告不会识别出你。如果你写信到下面的支持邮箱，开发者能看到的只有你自己写进那封邮件的内容。

## 儿童

本应用是面向专业人员的管理工具，并非面向儿童。它不向任何人收集信息，儿童亦然。

## 变更

若本政策发生变更，修订后的版本将发布在本网址，并标注新的生效日期。

## 联系方式

关于本政策，或关于本应用如何处理你的数据的任何疑问：**gaqo@outlook.com**

报告问题时，请**不要**附上密码、令牌，或应用存储文件夹中的文件。
