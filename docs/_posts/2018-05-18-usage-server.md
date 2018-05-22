---
layout: post
title:  服务端使用文档
categories: 教程
author: kongkongye
---

* content
{:toc}

主要给`服主`查阅,介绍如何在服务端安装与使用此菜单MOD对应的插件.




## 介绍
此菜单MOD有一个非常重要的特点,就是在客户端,它是一个`MOD`,而在服务端,它是一个`插件`(而非服务端MOD).

也就是说,你不需要开MOD服,也能使用此菜单MOD,如果你开了MOD服,那么装的也是插件.

即,不管插件服还是MOD服都能使用此菜单MOD,只要服务端装对应的插件即可.

## 下载
todo

## 前置需求

#### `java8`
如果你使用java7或更低的java版本来启动服务端,请升级到java8,
否则可能无法正常使用此菜单MOD.

#### `Vault`插件
其中`权限条件`,`无权限条件`需要使用Vault进行权限的检测.

[Vault下载](https://www.spigotmc.org/resources/vault.34315/)

#### `PlaceholderAPI`插件
也即常说的PAPI变量插件,`服务器全局变量`使用的就是此插件的变量.

[PlaceholderAPI下载](https://www.spigotmc.org/resources/placeholderapi.6245/)

## 安装
将下载的插件(以`jar`为后缀的文件)放入`plugins`文件夹

## 使用

#### 配置文件
安装后重启服务器,便会生成名为`MenuPlugin`的插件配置文件夹,可以自行修改配置.

如何重置配置文件?删除MenuPlugin文件夹,重启服务器或重载插件即可重新生成配置.

#### 命令
* `/MenuPlugin reload`: 重载配置(只能由控制台或OP玩家输入)

小提示: 命令`MenuPlugin`有个别名`mp`,因此`/MenuPlugin xxx`可以简化为`/mp xxx`
