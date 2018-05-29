---
layout: post
title:  内置变量
categories: 附录
author: kongkongye
---

* content
{:toc}

此篇文章仅在你需要修改此菜单MOD的默认内置菜单时需要.
详细列举了此菜单MOD提供了哪些本地全局/页面/列表变量,服务器页面/列表变量.
其它情况下你可以忽略此篇文章.




## 本地全局变量

#### MOD信息
变量类型为`MENU-ModInfo`,提供的本地全局变量值有:

* `name`: 此菜单MOD名
* `version`: 此菜单MOD版本
* `configFolder`: 此菜单MOD的配置目录的完整路径

#### 状态
变量类型为`MENU-status`,提供的本地全局变量值有:

* `connectServer`: true/false,是否连接上服务器

#### 管理菜单
变量名为`MENU-thirdMenusManage`,提供的本地全局变量值有:

* `hasWaiting`: 第三方菜单内是否有等待确认的菜单

## 本地页面变量

#### 主题
变量类型为`MENU-theme`,提供页面变量:

* `currentThemeId`: 当前选择的主题id
* `showThemeName`: 当前使用的主题名
* `serverThemeName`: 服务器主题名

#### 第三方命名空间
变量类型为`MENU-thirdNamespace`,需要输入变量:

* `namespace`: 命名空间名

提供页面变量:

* `namespace`: 命名空间
* `status`: 状态
    * `enabled`: 已启用
    * `waiting`: 等待确认
    * `disabled`: 已禁用
* `hasAttach`: 是否有附属
* `name`: 第三方命名空间名称,可为空
* `description`: 第三方命名空间描述,可为空
* `version`: 第三方命名空间版本,可为空
* `author`: 第三方命名空间作者,可为空
* `website`: 第三方命名空间网站,可为空

## 本地列表变量

#### 第三方主题
提供主题的相关信息,变量类型为`MENU-thirdThemes`,提供列表变量:

* `id`: 主题id
* `name`: 主题名

#### 所有的本地+第三方入口菜单
提供所有本地与第三方命名空间的入口菜单的相关信息,变量类型为`MENU-localMenus`,提供列表变量:

* `repo`: 仓库
* `namespace`: 命名空间
* `path`: 路径
* `title`: 菜单标题

#### 指定命名空间内的第三方入口菜单
提供入口菜单的相关信息,变量类型为`MENU-thirdIndexMenus`,需要输入变量:

* `namespace`: 命名空间名

提供列表变量:

* `repo`: 仓库(在这里值为`third`)
* `namespace`: 命名空间
* `path`: 路径
* `title`: 菜单标题

#### 第三方菜单管理内的命名空间列表
变量类型为`MENU-thirdMenusManage`,提供列表变量:

* `namespace`: 命名空间
* `status`: 状态
    * `enabled`: 已启用
    * `waiting`: 等待确认
    * `disabled`: 已禁用
* `hasAttach`: 是否有附属
* `name`: 第三方命名空间名称,可为空
* `description`: 第三方命名空间描述,可为空
* `version`: 第三方命名空间版本,可为空
* `author`: 第三方命名空间作者,可为空
* `website`: 第三方命名空间网站,可为空

## 服务器页面变量
无

## 服务器列表变量

#### 所有的服务器入口菜单
变量类型为`MENU-main`,提供列表变量:

* `namespace`: 命名空间
* `path`: 路径
* `title`: 菜单标题
