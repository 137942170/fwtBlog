---
layout: post
title: test
date: 2019-06-21 14:02:50
comments: true
tags:
- 标签1

---

### 引用块

{% blockquote [author[, source]] [link] [source_link_title] %}
content
{% endblockquote %}

### 样例

{% blockquote %}
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque hendrerit lacus ut purus iaculis feugiat. Sed nec tempor elit, quis aliquam neque. Curabitur sed diam eget dolor fermentum semper at eu lorem.
{% endblockquote %}

### 引用书上的句子

{% blockquote David Levithan, Wide Awake %}
Do not just seek happiness for yourself. Seek happiness for all. Through kindness. Through mercy.
{% endblockquote %}

### jsFiddle

#### 在文章中嵌入 jsFiddle

{% jsfiddle shorttag [tabs] [skin] [width] [height] %}

#### 在文章中插入指定大小的图片。

{% img [class names] /path/to/image [width] [height] [title text [alt text]] %}
