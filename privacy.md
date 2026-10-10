---
title: Privacy Policy
---

# Privacy Policy — Portal One For ArcGIS

**Effective 24 September 2026.** Portal One For ArcGIS was previously called AGOL-Enterprise
Admin Kit; this policy covers it under either name.

## The short version

This application collects nothing. It has no analytics, no telemetry, and no
crash reporting service. Nothing about you, your organization, or your use of
the application is sent to the developer or to any third party — not on first
run, not on failure, not ever.

The application talks to one kind of server: the ArcGIS Online or ArcGIS
Enterprise portal whose address **you** enter. Everything it produces stays on
your computer.

## What the application stores, and where

All of it lives in the application's own folder on your computer, under
`%LOCALAPPDATA%\Packages\`. None of it is uploaded anywhere.

| File | What it holds |
| --- | --- |
| `tokens.dat` | Sign-in tokens for the portals you connect to |
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

Passwords are never written to disk. When you choose to stay signed in, the
application saves the portal's token, not your password.

### About the logs

`activation.log` and `crash.log` record names, counts and error types — for
example "member list read, members=5". They do not record passwords, tokens, or
the contents of your data. They are never transmitted. You can delete them at
any time.

## What the application sends, and to whom

Only to the portal you are signed in to, and only the requests needed to do
what you asked: listing content, reading item details, transferring ownership,
deleting an item you selected. Those requests carry your access token in an
authorization header so the portal knows who is asking.

The application will also contact `www.arcgis.com` when you connect to ArcGIS
Online, because that is where ArcGIS Online lives.

There is no other network destination. There is no developer server.

## What the developer can see

Nothing. There is no account, no registration, and no server to collect
anything. If you write to the support address below, the developer sees only
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

**生效日期：2026 年 9 月 24 日**。Portal One For ArcGIS 原名 AGOL-Enterprise Admin Kit，本政策对两个名称同样适用。

## 一句话版本

本应用**不收集任何数据**。没有分析统计，没有遥测，没有崩溃上报服务。关于你、你的组织、你如何使用本应用的任何信息，都不会发送给开发者或任何第三方——首次运行时不会，出错时不会，任何时候都不会。

本应用只与一类服务器通信：**你自己填写地址**的 ArcGIS Online 或 ArcGIS Enterprise 门户。它产生的一切都留在你自己的电脑上。

## 本应用保存什么，保存在哪

全部位于本机 `%LOCALAPPDATA%\Packages\` 下应用自己的文件夹内，不会上传到任何地方。

| 文件 | 内容 |
| --- | --- |
| `tokens.dat` | 你所连接门户的登录令牌 |
| `portals.json` | 你添加的门户地址与显示名称 |
| `offboarding-journal.json` | 你执行过的转移与删除记录，用于复查和撤销 |
| `acknowledged-findings.json` | 你已标记为"已查看"的审计发现项 |
| `activation.log` | 应用的启动时间，以及扫描到的条目数量 |
| `crash.log` | 仅在应用意外失败时写入 |

### 关于你的凭据

登录令牌使用 Windows 数据保护 API 加密，作用域绑定到你的 Windows 用户账号。同一台电脑上的其他用户无法读取，复制到另一台机器也无法解密。如果你通过浏览器窗口登录，Microsoft Edge WebView2 会在同一个应用文件夹内保存它自己的会话数据。

**密码从不写入磁盘。** 当你选择保持登录时，应用保存的是门户返回的令牌，不是你的密码。

### 关于日志

`activation.log` 和 `crash.log` 只记录名称、数量和错误类型——例如"成员列表已读取，成员数=5"。它们**不记录**密码、令牌或你的数据内容，也从不传输。你可以随时删除它们。

## 本应用向谁发送什么

只发送给你已登录的那个门户，且只发送完成你所要求的操作所必需的请求：列出内容、读取条目详情、转移归属、删除你选中的条目。这些请求在授权头中携带你的访问令牌，以便门户识别请求者身份。

当你连接 ArcGIS Online 时，应用还会访问 `www.arcgis.com`，因为那就是 ArcGIS Online 所在之处。

除此之外没有任何其他网络目的地，**不存在开发者服务器**。

## 开发者能看到什么

什么也看不到。本应用没有账号体系、无需注册，也不存在任何用于收集信息的服务器。如果你写信到下面的支持邮箱，开发者能看到的只有你自己写进那封邮件的内容。

## 儿童

本应用是面向专业人员的管理工具，并非面向儿童。它不向任何人收集信息，儿童亦然。

## 变更

若本政策发生变更，修订后的版本将发布在本网址，并标注新的生效日期。

## 联系方式

关于本政策，或关于本应用如何处理你的数据的任何疑问：**gaqo@outlook.com**

报告问题时，请**不要**附上密码、令牌，或应用存储文件夹中的文件。
