# GitBook

## The new version is up! 老版本不再支持注册
旧地址 https://legacy.gitbook.com ==> 新地址 https://www.gitbook.com
![gitbook_new_version](/image/gitbook_new_version.png)

## GitBook 的目录结构
```
.
├── SUMMARY.md 定义目录结构，必选
├── README.md 说明，必选
├── book.json 插件，可选
├── GLOSSARY.md 要注释的术语列表，可选
├── .gitignore 或者.bookignore或者.ignore，编译的时候忽略的文件，可选
├── chapter-1/ 
|   ├── README.md
|   └── something.md
└── chapter-2/
    ├── README.md
    └── something.md
```
### Summary格式
```
# Summary

## Part I
* [Introduction](README.md)
    * [Writing is nice](part1/writing.md)
    * [GitBook is nice](part1/gitbook.md)

## Part II
* [We love feedback](part2/feedback_please.md)
* [Better tools for authors](part2/better_tools.md)
```

### book.json

### GitBook 可以生成一个网站，也可以生成电子书（ePub，Mobi，PDF），需要提前安装Calibre软件

```
# Generate a PDF file
$ gitbook pdf ./ ./mybook.pdf

# Generate an ePub file
$ gitbook epub ./ ./mybook.epub

# Generate a Mobi file
$ gitbook mobi ./ ./mybook.mobi
```

### 封面
- 可以使用 autocover plugin 生成一个。
- 自定义封面，cover.jpg 文件放在书本的根目录下。添加一个 cover_small.jpg 将指定一个较小版本的封面。封面应为 JPEG 文件。
好的封面应该遵守以下准则：
cover.jpg 的尺寸为 1800x2360 像素，cover_small.jpg 为 200x262
没有边界
清晰可见的书名
任何重要的文字应该在小版本中可见
