# DDD-Generator Framework

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/8treenet/gotree/blob/master/LICENSE) [![Go Report Card](https://goreportcard.com/badge/github.com/8treenet/freedom)](https://goreportcard.com/report/github.com/8treenet/freedom) [![Build Status](https://travis-ci.org/8treenet/gotree.svg?branch=master)](https://travis-ci.org/8treenet/gotree) [![GoDoc](https://godoc.org/github.com/8treenet/freedom?status.svg)](https://godoc.org/github.com/8treenet/freedom)
[![GitHub release](https://img.shields.io/github/v/release/8treenet/freedom.svg)](https://github.com/8treenet/freedom/releases)
<img align="right" width="200px" src="https://raw.githubusercontent.com/8treenet/blog/master/img/freedom.png">
###### ddd-generator是一个基于六边形架构的框架，可以支撑充血的领域模型范式。

## Overview
- 基于toml文件格式的领域描述语言
- 集成Iris v12 & Beego v2 & Gin
- 集成普罗米修斯
- 无侵入式Trace
- 基于组件式的 Infrastructure
- HTTP/H2C Server & Client
- 依赖注入 & 依赖倒置
- CRUD & PO Generate
- DDD & 六边形架构
- 领域事件 & MQ组件
- CQRS & 聚合根 & 防腐层
- 一级缓存 & 二级缓存 & 防击穿
- 基于AST（抽象语法树分析）的代码修改
- GraphQL API

## 安装
```sh
$ go get github.com/stevechan1993/ddd-generator
```

## 脚手架创建项目
```sh
$ ddd-generator new-project [project-name]
```

## 脚手架生成增删查改和持久化对象
####
```sh
# ddd-generator new-po -h 查看更多
$ cd [project-name]

# 数据库数据源方式
$ ddd-generator new-po --dsn "root:123123@tcp(127.0.0.1:3306)/freedom?charset=utf8"

# JSON 数据源方式
$ ddd-generator new-po --json ./domain/po/shcema.json
```

## Example

#### [基础教程](https://github.com/8treenet/freedom/blob/master/example/base)
#### [http2监听和依赖倒置](https://github.com/8treenet/freedom/blob/master/example/http2)
#### [事务组件&自定义组件&Kafka&领域事件组件](https://github.com/8treenet/freedom/blob/master/example/infra-example)

#### [一个完整的电商demo,包含CQS、聚合、实体、领域事件、资源库、基础设施](https://github.com/8treenet/freedom/blob/master/example/fshop)

