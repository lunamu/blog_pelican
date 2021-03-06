Title: 使用Pelican搭建静态博客
Date: 2014-05-16
Category: Pelican 
Tags: pelican, blog
Author: Lunamos


> “为什么总是忘记？因为缺乏真正的写作。”

> “请找一个拥有独立博客的男友。”

最近对于搭建静态博客并展示学习和制作内容的愿望比较强烈，因为只有通过自己加工思考并输出的内容才能够真正成为自己的。目前希望能够有支持Markdown等语法的静态博客生成器制作静态博客。在网上调研一番，主要有以下几种：

- Jekyll，使用Ruby编写，静态生成支持Markdown等语法的静态站点，但速度较慢，而且需要安装Ruby环境等。
- Hexo，使用Node.js，速度较快。
- Pelican，类似Jekyll，使用Python编写，较亲近一些。

其他没有选择的途径：

- Farbox，使用Dropbox作为博客托管站点，问题是需要付费，同时团队称可能产品无法维系太长时间，故作罢。
- Wordpress，基于PHP，动态站点，过于庞大。以后可能考虑自己编写博客框架。

Github为每一个用户分配了一个二级域名username.github.io，用户为自己的二级域名创建主页很简单，只需要在Github下创建一个名为username.github.io的版本库，并向其master分支提交网站静态页面即可。
由于Github的方便，因此目前选择Pelican，今后可能考虑移植到Hexo下。

## 准备

Pelican的[中文文档](https://pelican-docs-chs.readthedocs.org/en/latest/)。
Pelican的[英文文档](http://docs.getpelican.com/en/latest/)。

通过研读Pelican的英文文档，获知其部署方法。安装Python2.7或3.3/3.4之后，安装pip。
下载[get-pip.py](https://bootstrap.pypa.io/get-pip.py)，运行:
```bash
python get-pip.py
```
之后执行pip看是否安装成功。如果显示了ImportError: DLL load failed: %1 不是有效的 Win32 应用程序。
表明混用了64位的Python解释器和32位的package，或者相反。

之后安装pelican和markdown：
```bash
pip install pelican markdown
```


# 使用快速部署
进入博客/网站的目录，通过pelican-quickstart对项目进行快速部署。


Windows下Markdown编辑器 的选择：[Cmd Markdown](https://www.zybuluo.com/mdeditor)。

