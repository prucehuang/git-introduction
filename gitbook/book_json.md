# book插件

## book.json demo
```
{
    "title": "Git-Introduction",
    "description": "GitHub、GitBook简单使用介绍",
    "language": "zh-hans",
    "gitbook": "3.2.3",
    "styles": {
        "website": "./styles/website.css"
    },
    "structure": {
        "readme": "README.md"
    },
    "links": {
        "sidebar": {
            "GitHub地址": "https://github.com/prucehuang/git-introduction.git" 
        }
    },
    "author": "pruce",
    "plugins": [
        "back-to-top-button",
        "splitter",
        "expandable-chapters-small",
        "-sharing",
        "search-pro",
        "tbfed-pagefooter",
        "advanced-emoji",
        "github",
        "donate",
        "multipart"
    ],
    "pluginsConfig": {
        "theme-default": {
            "showLevel": true
        },
        "tbfed-pagefooter": {
            "copyright": "Copyright (c) 2018 Tencent PRUCE & MG.",
            "modify_label": "time：",
            "modify_format": "YYYY-MM-DD HH:mm:ss"
        },
        "github": {
            "url": "https://github.com/prucehuang/gitbook-introduction"
        },
        "donate": {
            "wechat": "https://github.com/prucehuang/common-resources/blob/master/pictures/wechat_pay.jpg?raw=true",
            "alipay": "https://github.com/prucehuang/common-resources/blob/master/pictures/zhifubao_pay.jpg?raw=true",
            "title": "",
            "button": "赏",
            "alipayText": "支付宝打赏",
            "wechatText": "微信打赏"
        }
    },
    "pdf": {
        "chapterMark": "pagebreak",
        "fontFamily": "Arial",
        "fontSize": 16,
        "margin": {
            "bottom": 56,
            "left": 62,
            "right": 62,
            "top": 56
        },
        "pageBreaksBefore": "/",
        "pageNumbers": true,
        "paperSize": "a4"
    }
}
```
## 常规配置

变量 | 说明
---|---
root | 包含所有图书文件的根文件夹的路径，除了 book.json
title | 书名
description | 书籍的描述
author | 作者名
isbn | 国际标准书号 ISBN
language | 本书的语言类型 —— ISO code 。默认值是 en
direction | 文本阅读顺序。可以是 rtl （从右向左）或 ltr （从左向右），默认值依赖于 language 的值。
gitbook | 应该使用的GitBook版本。使用 SemVer 规范，并接受类似于 “> = 3.0.0” 的条件。

## 不常规配置
1. links 在左侧导航栏添加链接信息
```
"links" : {
    "sidebar" : {
        "Home" : "https://github.com/dunwu/gitbook-notes"
    }
}
```

2. styles 自定义页面样式
默认情况下各generator对应的css文件
```
"styles": {
    "website": "styles/website.css",
    "ebook": "styles/ebook.css",
    "pdf": "styles/pdf.css",
    "mobi": "styles/mobi.css",
    "epub": "styles/epub.css"
}
例如要使 h1、h2 标签有下边框， 可以在 website.css 中设置
h1 , h2{
    border-bottom: 1px solid #EFEAEA;
}
```

3. plugins
- plugins 要加载的插件列表
- pluginsConfig 插件的配置  

```
Gitbook 默认带有 5 个插件：

highlight
search
sharing
font-settings
livereload

# 去除自带插件
"plugins": [
    "-search"
]
# 添加插件
"plugins": [
    "splitter"
]
配置完后执行
$ gitbook install
```





structure
除了 root 属性之外，您可以指定 Readme，Summary，Glossary 和 Languages 的名称（而不是使用默认名称，如README.md）。这些文件必须在项目的根目录下（或 root 的根目录，如果你在 book.json 中配置了 root 属性）。不接受的路径，如：dir / MY_README.md。
变量
描述
structure.readme
Readme 文件名（默认值是 README.md ）
structure.summary
Summary 文件名（默认值是 SUMMARY.md ）
structure.glossary
Glossary 文件名（默认值是 GLOSSARY.md ）
structure.languages
Languages 文件名（默认值是 LANGS.md ）
pdf
可以使用 book.json 中的一组选项来定制PDF输出：
Variable
Description
pdf.pageNumbers
将页码添加到每个页面的底部（默认为 true）
pdf.fontSize
基本字体大小（默认是 12）
pdf.fontFamily
基本字体样式（默认是 Arial）
pdf.paperSize
页面尺寸，选项有： 'a0', 'a1', 'a2', 'a3', 'a4', 'a5', 'a6', 'b0', 'b1', 'b2', 'b3', 'b4', 'b5', 'b6', 'legal', 'letter' （默认值是 a4）
pdf.margin.top
上边界（默认值是 56）
pdf.margin.bottom
下边界（默认值是 56）
pdf.margin.right
右边界（默认值是 62）
pdf.margin.left
左边界（默认值是 62）
Copyright © Zhang Peng 2017 all right reserved，powered by Gitbook
文件最近一次修订时间： 2017-11-10 02:40:04 

赏



