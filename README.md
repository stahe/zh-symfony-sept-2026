# [Symfony] Web 框架分步入门

**课程在线阅读地址：[https://stahe.github.io/zh-symfony-sept-2026/](https://stahe.github.io/zh-symfony-sept-2026/)**

## 作者

本课程及其全部代码由 Anthropic 的 AI **Claude** 编写，Claude 是**唯一作者**，应 Serge Tahé 的请求完成（2026 年 9 月）。

## 概述

本课程循序渐进地指导你使用 **Symfony 8.1** 框架和 **PHP 8.4** 语言构建 MVC Web 应用。HTML 页面由服务器通过 **Twig** 视图生成，不使用客户端 JavaScript 框架。数据访问通过 **Doctrine** ORM 完成。

它改编自课程[[Laravel](https://stahe.github.io/zh-laravel-sept-2026/) Web 框架分步入门]——后者本身又基于 [Flask](https://stahe.github.io/zh-flask-sept-2026/)、[Spring MVC](https://stahe.github.io/zh-springmvc-sept-2026/)、[ASP.NET Core MVC](https://stahe.github.io/zh-aspnetcoremvc-sept-2026/) 和 [NestJS](https://stahe.github.io/zh-nestjs-html-sept-2026/) 的课程。这些示例编号相同、主题相同：你可以逐个示例地比较各个框架。

## 内容

| 章节 | 主题 | 示例 |
|---|---|---|
| 动作、路由、响应 | 路由（`#[Route]`）、控制器、响应、重定向、服务容器 | 01 至 06 |
| 动作模型 | 请求参数、参数解析器、验证约束、POST 请求 | 07–12 |
| 视图及其模型 | Twig、模板、宏、扩展、Form 组件、验证、Post/Redirect/Get、CSRF 防护 | 13–21 |
| 国际化 | 法语和英语应用（YAML 字典、ICU 消息） | 22 |
| 数据作用域 | 请求、会话、缓存、Cookie | 23 |
| 请求生命周期 | 核心事件、监听器、参数解析器、错误页面 | 24 |
| 身份验证与授权 | 防火墙、存放在 Cookie 中的 JWT 认证器、角色、验证码、速率限制 | 25–27 |
| 分层架构 | 使用 Doctrine 和 MySQL 的 Web / 业务逻辑 / DAO | 28 |
| 案例研究 | **RdvMedecins**，一个医疗预约安排应用，逐个文件讲解 | - |

`rdvmedecins2-symfony` 案例研究管理三种角色（管理员、医生、患者）：日历、预约、医生和客户管理、受验证码保护的账户创建，以及法语/英语界面。它使用与该应用其他版本相同的 `dbrdvmedecins2` 数据库。

## 先决条件

- PHP 8.4 或更高版本（扩展 `intl`、`mbstring`、`openssl`、`pdo_mysql`）；
- Composer 2；
- MySQL 8 或 MariaDB（Windows 上的 Laragon）；
- Visual Studio Code，以及 PHP Intelephense、Twig Language 2 和 YAML 扩展；
- curl。

源代码可从课程网站下载。其中不包含 `vendor` 文件夹：`composer install` 会创建它们——一个在 `exemples` 文件夹中，一个在 `rdvmedecins2-symfony` 文件夹中。
