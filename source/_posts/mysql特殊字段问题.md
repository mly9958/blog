---
title: Mysql中数据表特殊字段问题
date: 2020-1-3
categories:
- mysql
tags:
- mysql
- 特殊字段
---

最近在工作写代码的时候，使用springdatajpa向数据库插入数据时，怎么都插入不进去，一直报语法错误，我检查了字段类型，字段名称，都没有问题。

最后在网上查阅资料时发现，我数据库表有个字段名称为`desc`，这个名称和mysql数据库关键字冲突了，导致一直报错，更改为`description`后正常