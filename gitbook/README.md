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