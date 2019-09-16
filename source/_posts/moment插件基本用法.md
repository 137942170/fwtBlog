---
title: moment 插件基本用法
date: 2019-09-01 10:15:21
categories: 
    - JS插件
tags: 
    - JS时间插件
---

### 格式化日期

##### 当前时间:

```
    moment().format('YYYY-MM-DD HH:mm:ss');
```
##### 当前日期:

```
    moment().format('d');
```

##### 转换当前时间的Unix时间戳:

```
    moment().format('X'); 
```

### 相对时间

##### 20170901相对当前日期是2年前

```
    moment("20170901", "YYYYMMDD").fromNow();

```