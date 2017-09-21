# MDwiki 文档

## 搭建本地“MDwiki”

[]()

## 部署设置

- 初始化本地仓库

```bash
$ cd mdwiki
$ git init
```

- 创建分支并初始化提交

```bash
$ git checkout -b gh-pages
$ git add .
$ git commit -m "initial"
```

- 在“github”初始化一个仓库“mdwiki”

- 添加远程地址

```bash
$ git remote add origin git@github.com:[username]/mdwiki.git
$ git push -u origin gh-pages
```

- 在github上“setting”中查看"pages"设置发布"gh-pages"

- 设置成功，"mdwiki"就会发布在`username.github.io/mdwiki`


## MarkDown语法

## 生成网页

## 添加导航栏

创建`navigation.md`文件，放置于同`mdwiki.html`一个目录下，如下制作菜单：

```markdown
# Your wiki name

[Home](home.md)
[About](about.md)
[Download](download.md)
```

对于更复杂的菜单——有多个项目的可收缩子菜单，如下使用列表和水平线分隔显示：

```markdown
# Your wiki name

[菜单-1]()

  * # 子菜单-1
  * [子菜单 项目1-1](项目1-1.md)
  * [子菜单 项目1-2](项目1-2.md)
  ----
  * # 子菜单-2
  * [子菜单 项目2-1](项目2-1.md)
  * [子菜单 项目2-2](项目2-2.md)
  ----
  * # 子菜单-3
  * [子菜单 项目3-1](项目3-1.md)
  * [子菜单 项目3-2](项目3-2.md)

[菜单-2](菜单-2.md)
[菜单-3](菜单-3.md)

```

注意：

- 如果希望点击“菜单-1”展开列表，则“菜单-1”后面括号需要留空
- 子菜单标题前使用“#”，子菜单之间使用“----”水平线隔开
- 一级菜单之间，如果有子菜单，需要和其他一级菜单之间留空行

## 创建连接

- 链接到外部网站

```markdown
[Google](http:www.google.com)
```

- 链接到内部文件

```markdown
[下载](download.md)
```

## 图片

```markdown
![图片](图片放置位置或链接)
```

注意：如果想以图片组的形势呈现图片，可以用空行进行分组

```markdown
！[图片](路径或链接)

！[图片](路径或链接)
！[图片](路径或链接)

！[图片](路径或链接)
！[图片](路径或链接)
！[图片](路径或链接)
```

上面代码，呈现的是一个单独图片，两个一组的图片，三个一组的图片

### 图片链接

```markdown
[![图片](图片放置位置路径或链接)](图片链接到的地址)
```

注意： 图片链接，就连接的语法将图片的语法标记都包裹起来

## 语法高亮

支持的语法：

Language|keyword
:-:|:-:
Bash|bash
C#|csharp
Clojure|clojure
C++|cpp
CSS|css
CoffeeScript|coffeescript
CMake|cmake
HTML|html
HTTP|http
Java|java
JavaScript|javascript
JSON|json
Markdown|markdown
Objective C|objectivec
Perl|perl
PHP|php
Python|python
Ruby|ruby
R|r
SQL|sql
Scala|scala
Vala|vala
XML|xml




