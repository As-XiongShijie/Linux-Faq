Debian中的 *copyright(版权)*    *changlog(修订记录)*  都是可以删除的 没什么实际用途 但是不代表你能删除 请尊重别的的版权和劳动成果

![image-20210128184603626](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128184603626.png)

解读：

Source 是软件包的源代码名称 一般建议不要修改 否则别人如果不知道你设置的名称是什么可能会出现问题

Section 是软件类别  一般为 utils, net, mail, text, x11 这里是admin 管理员

Priority 软件对系统的重要程度 一般为  required, standard, optional, extra等 这里是optional 可以选择的 就是可以不要的东西 但是介于这个是控制中心 很多新手用户需要用Gui界面进行控制 我觉得这个还是需要的。

Maintainer 是维护者 这个地方显而易见 不用过多解释了

然后Build-Depends 是构建的依赖 下面还有很多东西 这里截屏只有一部分

![image-20210128185331117](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128185331117.png)

Standards-version 标准版本号 也就是软件的版本号

Homepage 主页 这里显示的是它在GitHub上的位置

Package	是程序名称而且中间不能有空格。所以它采用 “- ”来连接

Architecture	是软件所支持的平台架构	i386, amd64, m68k, sparc, alpha, powerpc等

这里是any 所有的都支持？

Depends	软件所依赖的其他软件包和库文件

Recommends	推荐安装的其他软件包和库文件

Suggests	建议安装的其他软件包和库文件

Conflicts 冲突 replaces 替代品 这个地方的天气插件和通知插件舒适没看懂

 Description	程序说明

下同







![image-20210128193253116](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128193253116.png)

 首先 我们先输入

`sudo apt-get install build-essential`

安装最基本的工具 如上图所示

![image-20210128193624754](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128193624754.png)

 输入以下命令查看是否安装了GTK：

`pkg-config --list-all | grep gtk`

由于我们这是新装的系统 自然什么都没有安装

安装GTK的命令：

sudo apt-get install gnome-devel gnome-devel-docs

![image-20210128194201331](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128194201331.png)

安装好之后输入： 

![image-20210128194738852](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128194738852.png)

`pkg-config --modversion gtk+-3.0`

查看gtk的版本。

![image-20210128194834078](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128194834078.png)

同样输入之前的命令也可以看到我们安装的一些东西

![image-20210128195516284](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128195516284.png)

我们尝试安装librsvg 发现已经有源里的最新版本了

![image-20210128195859484](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128195859484.png)

安装libcanberra

![image-20210128195948331](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128195948331.png)

有以上提示 不过我选择了继续安装

尝试安装poppler-glib

![image-20210128200204675](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128200204675.png)

安装libsqlite3:

![image-20210128200409499](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128200409499.png)

![image-20210128200448142](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128200448142.png)

至此

![image-20210128200544104](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128200544104.png)

以上内容都应该安装完成了



![image-20210128200941905](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128200941905.png)

用git 吧xcur2png 拉到本地

![image-20210128201206611](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128201206611.png)

![image-20210128201640425](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128201640425.png)

如图安装xcur2png 

![image-20210128201712028](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128201712028.png)

查看他的版本

![image-20210128202235176](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128202235176.png)

如图安装Go语言

![image-20210128213356241](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128213356241.png)

![image-20210128213418900](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128213418900.png)

如图操作

![image-20210128214704299](https://gitee.com/xiongshijie/xiongshijie2/raw/master/img/image-20210128214704299.png)

安装Gio-2.0