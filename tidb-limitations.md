---
title: TiDB 使用限制
category: introduction
---

# 使用限制

本文会将详细描述 TiDB 中常见的使用限制，包括：标识符长度，最大支持的数据库、表、索引、分区表、序列等的个数

## 标识符长度限制

| 标识符类型 | 最大长度（字符）|
|:---------|:--------------|
| Database | 64 |
| Table    | 64 |
| Cloumn   | 64 |
| Index    | 64 |
| View     | 64 |
| Sequence | 64 |

## Databases、Tables、Views、Connections 总个数限制

| 标识符类型  | 最大个数   |
|:----------|:----------|
| Databases | unlimited |
| Tables    | unlimited |
| Views     | unlimited |
| Connections| unlimited|


## 单个 Database 的限制

| 类型       | 最大限制   |
|:----------|:----------|
| Tables    |unlimited  |

## 单个 Table 的限制

| 类型       | 最大限制   |
|:----------|:----------|
| Cloumns   | 512       |
| Indexs    | 64        |
| Rows      | unlimited |
| Size      | unlimited |
| Partitions| 1024      |

## 单行的限制

| 类型       | 最大限制   |
|:----------|:----------|
| Sze       | 6MB       |

## 单列的限制

| 类型       | 最大限制   |
|:----------|:----------|
| Sze       | 6MB       |

## 字符串类型限制

| 类型       | 最大限制   |
|:----------|:----------|
| CHAR       | 256 字符      |
| BINARY     | 256 字节      |
| VARBINARY  | 65535 字节    |
| VARCHAR    | 16383 字符    |
| TEXT       | 6MB 字节      |
| BLOB       | 6MB 字节      |

## SQL Statements 的限制

| 类型       | 最大限制   |
|:----------|:----------|
| 单条 INSERT statement 语句写入的 Key-Value 对数量       |  3000000      |
| 单个事务写入的行数       |  3000000 / 单个表索引的数量      |
| 单条 INSERT statement 语句写入的 Key-Value 对数量       |  3000000      |
| 单个事务写入的行数       |  3000000 / 单个表索引的数量      |