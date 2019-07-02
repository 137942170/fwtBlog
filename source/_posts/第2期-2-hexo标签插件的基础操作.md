---
title: 第2期:(2)hexo标签插件的基础操作
date: 2019-07-01 12:18:52
tags:
    -md语法
    -7月
---

### hexo标签插件的基础操作

### 一、引用块

#### 1、普通输出

{% blockquote %}
    小时候枕头上都是口水，长大以后枕头上都是泪水，小时候微笑是一种心情，长大后微笑是一种表情，小时候哭着哭着就笑了，长大后笑着笑着就哭了我们终于到了小时候最羡慕的年纪，但却没能成为小时候最想成为的人
{% endblockquote %}

#### 2、引用书上的句子

{% blockquote fwt, Feng Feng %}
    小时候枕头上都是口水，长大以后枕头上都是泪水，小时候微笑是一种心情，长大后微笑是一种表情，小时候哭着哭着就笑了，长大后笑着笑着就哭了我们终于到了小时候最羡慕的年纪，但却没能成为小时候最想成为的人
{% endblockquote %}

#### 3、引用 Twitter

{% blockquote @DevDocs https://twitter.com/devdocs/status/356095192085962752 %}
NEW: DevDocs now comes with syntax highlighting. http://devdocs.io
{% endblockquote %}

#### 4、引用网络上的文章

{% blockquote Seth Godin https://137942170.github.io/fwtBlog/ Welcome to Island Marketing %}
小时候枕头上都是口水，长大以后枕头上都是泪水，小时候微笑是一种心情，长大后微笑是一种表情，小时候哭着哭着就笑了，长大后笑着笑着就哭了我们终于到了小时候最羡慕的年纪，但却没能成为小时候最想成为的人
{% endblockquote %}

### 二、代码块

#### 1、普通代码块

{% codeblock %}
alert('Hello javascript!');
{% endcodeblock %}

#### 2、指定语言

{% codeblock lang:objc %}
[rectangle setX: 10 y: 10 width: 20 height: 20];
{% endcodeblock %}

#### 3、附加内容

{% codeblock Array.map %}
array.map(callback[, thisArg])
{% endcodeblock %}

#### 4、附加网址

{% codeblock _.compact http://underscorejs.org/#compact Underscore.js %}
_.compact([0, 1, false, 2, '', 3]);
=> [1, 2, 3]
{% endcodeblock %}

### 三、反引号代码块

##### 由于此处加载大量网址 暂且不做示例

#### 1、Pull Quote
```
{% pullquote [class] %}
content
{% endpullquote %}
```
#### 2、jsFiddle
```
{% jsfiddle shorttag [tabs] [skin] [width] [height] %}
```
#### 3、Gist
```
{% gist gist_id [filename] %}
```
#### 4、iframe
```
{% iframe url [width] [height] %}
```
#### 5、Image
```
{% img [class names] /path/to/image [width] [height] [title text [alt text]] %}
```
#### 6、Link
```
{% link text url [external] [title] %}
```
#### 7、Include Code
```
{% include_code [title] [lang:language] path/to/file %}
```
#### 8、Youtube
```
{% youtube video_id %}
```
#### 9、Vimeo
```
{% vimeo video_id %}
```
### 四、引用文章
```
{% post_path slug %}
{% post_link slug [title] %}
```
### 五、引用资源
```
{% asset_path slug %}
{% asset_img slug [title] %}
{% asset_link slug [title] %}
```
### 六、Raw
```
{% raw %}
content
{% endraw %}
```