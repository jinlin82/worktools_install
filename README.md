---
title: "Worktools安装指南详细版"
author: "Jin's students"
date: "2019-11-23"
output:
  bookdown::html_document2:
    number_sections: true
    seq_numbering: true
    fig_caption: true
    highlight: haddock
    theme: null
    md_extensions: +east_asian_line_breaks
    keep_md: true
    toc: true
    pandoc_args: ["--filter", "pandoc-crossref", "-M", "eqnPrefix="]
  bookdown::word_document2:
    fig_caption: true
    reference_docx: ./style/word-styles-02.docx
    md_extensions: +east_asian_line_breaks
    pandoc_args: ["--filter", "pandoc-crossref"]
  bookdown::pdf_document2:
    keep_tex: yes
    toc: false
    latex_engine: xelatex
    md_extensions: +east_asian_line_breaks
    pandoc_args: ["--listing", "--filter", "pandoc-crossref"]
css: ./style/markdown.css
autoEqnLabels: true
eqnPrefixTemplate: ($$i$$)
linkReferences: true
bibliography: Bibfile.bib
csl: ./style/chinese-gb7714-2005-numeric.csl
link-citations: true
---


# Worktools安装指南详细版

1. 卸载电脑中已经安装的R和Rstudio和tex软件(包括 CTEX， Texlive等卸载干净，不要有R残留），接着重启电脑。
2. 把移动硬盘worktools文件夹里面的FastCopy211文件夹拷贝到桌面
3. 使用桌面FastCopy211文件夹里面的fastcopy.exe 把移动硬盘里面的 worktools 文件夹，
   texlive 文件夹和cygwin文件夹都拷贝至C盘根目录下（C盘至少有20个G剩余空间）
   （USB 3.0接口大约需要10分钟，USB 2.0接口大约需要60分钟）

![](./figure1.png)

4. 在C盘worktools文件夹中创建一个新的文件夹config
5. 点击RStudio-1.2.1335，将RStudio-1.2.1335安装到worktools文件夹中，点击RStudio-1.2.1335--bin--rstudio.exe,打开
界面如下：出现的是R version 3.5.1,进行下一步，如果出现的是其他版本的R,如3.6.1，则说明之前安装R没有卸载干净，
继续删除干净后，重启rstudio.exe，然后出现选择R版本的路径界面，选择C:\\Worktools\\R\\R-3.5.1，即可出现下图，关
联的是Worktools里的R-3.5.1

![](./figure2.png)

![](./figure3.png)

6. 安装anaconda3，直接安装在C盘，根目录下面(可在最后做）
7. 把C:\\Worktools\\Pandoc文件夹中的pandoc.exe，pandoc-citeproc.exe，pandoc-crossref.exe三个文件复制到C:\\Worktools
\\RStudio-1.2.1335\\bin\\pandoc 中，选择覆盖文件
8. 右键点击C:\\Worktools\\MobileWork中的run.bat，选择以管理员身份运行
9. 打开 C:\\Worktools\\Fonts 文件夹，全选里面所有文件，右键点击，选择安装
10. 重启rstudio,出现以下界面，说明安装完成

![](./figure4.png)

# Worktools 更新步骤
1. worktools文件名改为worktools.bak 
2. 把移动硬盘里面的worktools文件夹用fastcopy.exe拷贝到C盘根目录
3. 把 worktools.bak 里面的 config 文件夹复制到新的 worktools 里面
4. 测试，一个星期后没有问题就把worktools.bak删掉（需要30-60分钟） 
