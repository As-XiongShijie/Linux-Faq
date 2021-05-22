决定开个新贴来写关于texlive的使用历程吧！

首先就是他们的使用过程，配置环境 现在下面这个就是配置的过程 是在知乎上学的



## LaTeX环境的代码配置

## 6.1 LaTeX配置代码展示

先给出效果图：

![img](https://pic2.zhimg.com/80/v2-175b476a0cf425370065156bf807e205_720w.jpg)

LaTeX 配置代码如下（不包含外部 pdf 查看器设置）：

```json
{
    "latex-workshop.latex.autoBuild.run": "never",
    "latex-workshop.showContextMenu": true,
    "latex-workshop.intellisense.package.enabled": true,
    "latex-workshop.message.error.show": false,
    "latex-workshop.message.warning.show": false,
    "latex-workshop.latex.tools": [
        {
            "name": "xelatex",
            "command": "xelatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOCFILE%"
            ]
        },
        {
            "name": "pdflatex",
            "command": "pdflatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOCFILE%"
            ]
        },
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOCFILE%"
            ]
        },
        {
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
            ]
        }
    ],
    "latex-workshop.latex.recipes": [
        {
            "name": "XeLaTeX",
            "tools": [
                "xelatex"
            ]
        },
        {
            "name": "PDFLaTeX",
            "tools": [
                "pdflatex"
            ]
        },
        {
            "name": "BibTeX",
            "tools": [
                "bibtex"
            ]
        },
        {
            "name": "LaTeXmk",
            "tools": [
                "latexmk"
            ]
        },
        {
            "name": "xelatex -> bibtex -> xelatex*2",
            "tools": [
                "xelatex",
                "bibtex",
                "xelatex",
                "xelatex"
            ]
        },
        {
            "name": "pdflatex -> bibtex -> pdflatex*2",
            "tools": [
                "pdflatex",
                "bibtex",
                "pdflatex",
                "pdflatex"
            ]
        },
    ],
    "latex-workshop.latex.clean.fileTypes": [
        "*.aux",
        "*.bbl",
        "*.blg",
        "*.idx",
        "*.ind",
        "*.lof",
        "*.lot",
        "*.out",
        "*.toc",
        "*.acn",
        "*.acr",
        "*.alg",
        "*.glg",
        "*.glo",
        "*.gls",
        "*.ist",
        "*.fls",
        "*.log",
        "*.fdb_latexmk"
    ],
    "latex-workshop.latex.autoClean.run": "onFailed",
    "latex-workshop.latex.recipe.default": "lastUsed",
    "latex-workshop.view.pdf.internal.synctex.keybinding": "double-click"
}
```

**注 6 ：** 若您不想要配置外部查看器以及了解内部查看和外部查看之间切换操作，可以直接复制上述代码至 json 文件中，即可完成 LaTeX 的配置，从而可以对 LaTeX 代码进行编译。

**注 7 ：**根据 json 文件编写规则，每个代码语句（除了代码块儿最后一句）都需要加上英文状态下的`,`，否则就会报错；而每个代码块儿的最后一句是不需要加上`,`的。从上文整个代码块儿可以看出此规则。

如果您日后需要在上述代码之后再添加其他代码，请记得在最后一句

```json
"latex-workshop.view.pdf.internal.synctex.keybinding": "double-click"
```

后添加上`,`，即变为

```json
"latex-workshop.view.pdf.internal.synctex.keybinding": "double-click",
......
```

其中的`......`为您添加的其余代码。

**切记！**

## 6.2 LaTeX配置代码解读

如果您对此不感兴趣，可以跳过该小节。下面进行代码**注释解读**：

```json
"latex-workshop.latex.autoBuild.run": "never"
```

设置何时使用默认的(第一个)编译链自动构建 LaTeX 项目，即什么时候自动进行代码的编译。有三个选项： 

\1. **onFileChange**：在检测任何依赖项中的文件更改(甚至被其他应用程序修改)时构建项目，即当检测到代码被更改时就自动编译tex文件； 

\2. **onSave** : 当代码被保存时自动编译文件； 

\3. **never**:  从不自动编译，即需编写者手动编译文档

此项笔者设置为**never**。

```json
"latex-workshop.showContextMenu": true
```

启用上下文LaTeX菜单。此菜单默认状态下停用，即变量设置为**false**，因为它可以通过新的 LaTeX 标记使用（新的 LaTeX 标记能够编译文档，将在下文提及）。只需将此变量设置为**true**即可恢复菜单。即此命令设置是否将编译文档的选项出现在鼠标右键的菜单中。

下两图展示两者区别，第一幅图为设置**false**情况，第二幅图为设置**true**情况。可以看到的是，设置为**true**时，菜单中多了两个选项，其中多出来的第一个选项为进行tex文件的编译，而第二个选项为进行正向同步，即从代码定位到编译出来的 pdf 文件相应位置，下文会进行提及。 

![img](https://pic2.zhimg.com/80/v2-d614a4ecc4b7da18624926b5a49f144d_720w.jpg)

![img](https://pic3.zhimg.com/80/v2-c66892ca1a278e961fe9fdb124896126_720w.jpg)

 笔者觉得菜单多了此选项较方便，故此项笔者设置为**true**

```json
"latex-workshop.intellisense.package.enabled": true
```

设置为**true**，则该拓展能够从使用的宏包中自动提取命令和环境，从而补全正在编写的代码。

```json
"latex-workshop.message.error.show"  : false,
"latex-workshop.message.warning.show": false
```

这两个命令是设置当文档编译错误时是否弹出显示出错和警告的弹窗。因为这些错误和警告信息能够从终端中获取，且弹窗弹出比较烦人，故而笔者设置均设置为**false**。

```json
"latex-workshop.latex.tools": [
        {
            "name": "xelatex",
            "command": "xelatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOCFILE%"
            ]
        },
        {
            "name": "pdflatex",
            "command": "pdflatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOCFILE%"
            ]
        },
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOCFILE%"
            ]
        },
        {
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
            ]
        }
    ]
```

这些代码是定义在下文 recipes 编译链中被使用的编译命令，此处为默认配置，不需要进行更改。其中的`name`为这些命令的标签，用作下文 recipes 的引用；而`command`为在该拓展中的编译方式。

可以更改的代码为，将编译方式: pdflatex 、 xelatex 和 latexmk 中的`%DOCFILE`更改为`%DOC`。`%DOCFILE`表明编译器访问没有扩展名的根文件名，而`%DOC`表明编译器访问的是没有扩展名的根文件完整路径。这就意味着，使用`%DOCFILE`可以将文件所在路径设置为中文，但笔者不建议这么做，因为毕竟涉及到代码，当其余编译器引用时该 tex 文件仍需要根文件完整路径，且需要为英文路径。笔者此处设置为`%DOCFILE`仅是因为之前使用 TeXstudio，导致路径已经是中文了。

更多详情可以访问 github 中 LaTeX-Workshop 的 Wiki:  

[https://github.com/James-Yu/LaTeX-Workshop/wiki/Compile#placeholders](https://link.zhihu.com/?target=https%3A//github.com/James-Yu/LaTeX-Workshop/wiki/Compile%23placeholders)[github.com](https://link.zhihu.com/?target=https%3A//github.com/James-Yu/LaTeX-Workshop/wiki/Compile%23placeholders)

```json
"latex-workshop.latex.recipes": [        {            "name": "XeLaTeX",            "tools": [                "xelatex"            ]        },        {            "name": "PDFLaTeX",            "tools": [                "pdflatex"            ]        },        {            "name": "BibTeX",            "tools": [                "bibtex"            ]        },        {            "name": "LaTeXmk",            "tools": [                "latexmk"            ]        },        {            "name": "xelatex -> bibtex -> xelatex*2",            "tools": [                "xelatex",                "bibtex",                "xelatex",                "xelatex"            ]        },        {            "name": "pdflatex -> bibtex -> pdflatex*2",            "tools": [                "pdflatex",                "bibtex",                "pdflatex",                "pdflatex"            ]        }    ]
```

此串代码是对编译链进行定义，其中`name`是标签，也就是出现在工具栏中的链名称；`tool`是`name`标签所对应的编译顺序，其内部编译命令来自上文`latex-workshop.latex.recipes`中内容。

定义完成后，能够在 vscode 编译器中能够看到的编译顺序，具体看下图：

![img](https://pic2.zhimg.com/80/v2-42b419223d07a18fd406ecd54f674fd1_720w.jpg)

可以看到的是，在编译链中定义的命令出现在了vscode右侧的工具栏中。

**注 8 ：PDFLaTeX** 编译模式与 **XeLaTeX** 区别如下：

>  \1. PDFLaTeX 使用的是TeX的标准字体，所以生成PDF时，会将所有的非 TeX 标准字体进行替换，其生成的 PDF  文件默认嵌入所有字体；而使用 XeLaTeX 编译，如果说论文中有很多图片或者其他元素没有嵌入字体的话，生成的 PDF  文件也会有些字体没有嵌入。 
>
>  \2. XeLaTeX 对应的 XeTeX 对字体的支持更好，允许用户使用操作系统字体来代替 TeX 的标准字体，而且对非拉丁字体的支持更好。 
>
>  \3. PDFLaTeX 进行编译的速度比 XeLaTeX 速度快。

引用自 *蛐蛐蛐先生的博客* ：

[PDFLaTeX和XeLaTeX有什么区别_qysh123的专栏-CSDN博客_xelatex和pdflatex哪个更好](https://link.zhihu.com/?target=https%3A//blog.csdn.net/qysh123/article/details/11833649%3Futm_source%3Dtuicool)[blog.csdn.net![图标](https://pic1.zhimg.com/v2-2a5027b5bff83f50a189c6146b4f7548_ipico.jpg)](https://link.zhihu.com/?target=https%3A//blog.csdn.net/qysh123/article/details/11833649%3Futm_source%3Dtuicool)

**注 9 ：** 编译链的存在是为了更方便编译，因为如果涉及到**.bib**文件，就需要进行多次不同命令的转换编译，比较麻烦，而编译链就解决了这个问题。

```json
"latex-workshop.latex.clean.fileTypes": [        "*.aux",        "*.bbl",        "*.blg",        "*.idx",        "*.ind",        "*.lof",        "*.lot",        "*.out",        "*.toc",        "*.acn",        "*.acr",        "*.alg",        "*.glg",        "*.glo",        "*.gls",        "*.ist",        "*.fls",        "*.log",        "*.fdb_latexmk"    ]
```

这串命令则是设置编译完成后要清除掉的辅助文件类型，若无特殊需求，无需进行更改。

```json
"latex-workshop.latex.autoClean.run": "onFailed"
```

这条命令是设置什么时候对上文设置的辅助文件进行清除。其变量有： 

\1. **onBuilt** : 无论是否编译成功，都选择清除辅助文件； 

\2. **onFailed** : 当编译失败时，清除辅助文件； 

\3. **never** : 无论何时，都不清除辅助文件。

由于 tex 文档编译有时需要用到辅助文件，比如编译目录和编译参考文献时，如果使用`onBuilt`命令，则会导致编译不出完整结果甚至编译失败；

而有时候将 tex 文件修改后进行编译时，可能会导致 pdf 文件没有正常更新的情况，这个时候可能就是由于辅助文件没有进行及时更新的缘故，需要清除辅助文件了，而`never`命令做不到这一点；

故而笔者使用了`onFailed`，同时解决了上述两个问题。

```json
"latex-workshop.latex.recipe.default": "lastUsed"
```

该命令的作用为设置 vscode 编译 tex 文档时的默认编译链。有两个变量： 1. **first** :  使用`latex-workshop.latex.recipes`中的第一条编译链，故而您可以根据自己的需要更改编译链顺序； 2. **lastUsed** : 使用最近一次编译所用的编译链。

笔者选择使用**lastUsed**。

```json
"latex-workshop.view.pdf.internal.synctex.keybinding": "double-click"
```

用于反向同步（即从编译出的 pdf 文件指定位置跳转到 tex 文件中相应代码所在位置）的内部查看器的快捷键绑定。变量有两种： 

\1. **ctrl-click** ： 为默认选项，使用Ctrl/cmd+鼠标左键单击 

\2. **double-click** :  使用鼠标左键双击

此处笔者使用的为**double-click**。



**注 10 ：** 若因网络原因无法连接到github导致无法下载，可以使用自己的tex文件进行测试，或者复制以下代码进行文档的简单编译测试，但其只能测试一部分功能：

```tex
\documentclass[a4paper]{article}\usepackage[margin=1in]{geometry} % 设置边距，符合Word设定\usepackage{ctex}\usepackage{lipsum}\title{\heiti\zihao{2} This is a test for vscode}\author{\songti Ali-loner}\date{2020.08.02}\begin{document}    \maketitle\begin{abstract}    \lipsum[2]\end{abstract}\tableofcontents\section{This is a section}Hello world! 你好，世界 ！\end{document}
```

## 7.2  tex 测试文件编译

**① 打开测试文件所在文件夹**

![img](https://pic1.zhimg.com/80/v2-cc8b54b9dd5e44f7ff79b988c5d214d4_720w.jpg)

**② 点击选中 tex 文件**，进行文件内容查看

![img](https://pic4.zhimg.com/80/v2-2938ac1763f64723cc7f2812923ccf07_720w.jpg)

**③ 开始编译文件。** 由于进行测试的文件中涉及参考文献的引用（**.bib**的编译），故而选择`xelatex -> bibtex -> xelatex*2`编译链。

![img](https://pic3.zhimg.com/80/v2-c42deeda6c6dd52e46ca85f780d77a6e_720w.jpg)

**注 11 ：**为了更方便进行编译，可对其设置快捷键，设置快捷键步骤如下：

![img](https://pic2.zhimg.com/80/v2-f9c5c82990dbeac2895ec2593bbff1c5_720w.jpg)

笔者将快捷键设置为**Ctrl+Alt+R**。

**选中tex文件的代码页面**（若未选中，则无法进行编译），然后按下该快捷键，在编辑器页面上端进行编译链选择，如下图：

![img](https://pic3.zhimg.com/80/v2-c9fb99fa3eab73827ecfe822ea24f316_720w.jpg)

**④ 编译成功**

当发现页面下方出现 **√** 符号时，说明编译成功，相反，如果出现 **×** 符号，说明编译失败，就要找失败原因了。

**a.** 左侧工具栏

当编译成功后，选中 tex 文件中任意的代码，以此来选中 tex 文件，然后进行图示操作。其中侧边栏所展现的就是上文提及的新的 LaTeX 标记。

![img](https://pic3.zhimg.com/80/v2-7581b1033a9c201fc13c9c1ebb05d01e_720w.jpg)

**b.** 快捷键

选中 tex 文件中任意的代码，然后按**Ctrl+Alt+V**，出现编译好的 pdf 页面。该快捷键为默认设置。若您想要更改，可以根据上文进行配置。

![img](https://pic4.zhimg.com/80/v2-880a90f3a4feb0e1628d21b7765acaa3_720w.jpg)

注意到，现在编译的结果为内部查看器查看。

**⑤ 正向同步测试**，即从代码定位到 pdf 页面相应位置。有以下三种方法：

**a.** 使用侧边工具栏

![img](https://pic2.zhimg.com/80/v2-26481bfc0f4bccff10394e3746ad61e1_720w.jpg)

**b.** 使用右键菜单

![img](https://pic4.zhimg.com/80/v2-5f13291f73b7182ec16cfb5585d729f7_720w.jpg)

**c.** 使用快捷键

选中需要跳转的代码所在行，按Ctrl+Alt+J，右侧就会跳转到相应行。这里的快捷键为默认设置，可自行通过上文方式设置为您想要的快捷键。

**⑥ 反向同步测试**,即从 pdf 页面定位到代码相应位置

在编译生成的 pdf 上，选中想要跳转行，鼠标**左键双击**或**ctrl+鼠标左键单击**，跳转到对应代码。此处快捷键的选择为上文设置，若使用笔者的代码，则为**鼠标左键双击**。

![img](https://pic3.zhimg.com/80/v2-2297f86ee5e2ed18067fbbb82c6c539a_720w.jpg)

