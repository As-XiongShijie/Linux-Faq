**正题**

首先安装refind，安装方式异常简单。

```
sudo apt install refind  //安装这个包
sudo refind-install      //通过自带的安装脚本安装refind引导
```

此时操作完后需要打开bios设置界面，然后关闭安全启动即可。

重启就可以看到效果了。（至此就能正常使用了，是不是异常的简单）

**优化**

因为refind会在启动时扫描所有启动文件，所以你在开机的时候会看到大概5个启动项，其中有一个是Windows，其余全部是Linux，还有一个是Ubuntu，大部分都是Grub的引导，因为安全起见，我们并没有删除Grub，只是让bios启动时先加载refind罢了，如果你选择grub的启动项，会在refind菜单退出后进入grub菜单，这就有点脱裤子放屁的意思，而且开机速度肯定会变慢一些，即使在控制中心关闭启动延迟，也会加载grub。所以，我们需要屏蔽那些无用的启动项，只需一个Windows，一个Deepin即可。如果有兴趣可以美化一下。

**屏蔽多余启动项**

从文件管理器中打开“系统盘-->boot-->efi-->EFI-->refind”，然后右键用管理员身份打开此文件夹，此时双击打开refind.conf文件，弹出窗口时点击显示。

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=202011131347056413_thread_KaSQEDpqiGu.png)

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=202011131347323090_thread_Rk51ozuTqbT.png)

在此文件末尾添加以下内容，表示屏蔽扫描的文件夹启动项，用逗号隔开。

```
dont_scan_dirs ESP:/EFI/boot,EFI/ubuntu,EFI/boot,EFI/deepin_os,EFI/UOS
```

其中的boot，ubuntu，deepin_os，UOS都是grub的启动项，所以都屏蔽即可。

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=202011131349305194_thread_RKK9DPPKdsw.png)

这时点击保存重启后，应该只剩下Windows和deepin两个选项了。

**美化**

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=202011131447504078_thread_pX3sEhBDxiD.jpg)

这是网上找到的图，我就用的这个主题，大家喜欢的话就往下看。

https://github.com/EvanPurkhiser/rEFInd-minimal这时这个主题的项目地址。

往下看可以找到作者写的文档（希望大家在学习东西的时候，先看一下作者的文档，不懂的话再去百度寻找资料）

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=20201113135642563_thread_lKkWmCcxdrW.png)



你需要在刚刚那个refind所在的目录下新建一个文件夹，命名为themes,然后将这个主题文件夹复制进去

主题下载地址：

https://github.com/EvanPurkhiser/rEFInd-minimal/archive/master.zip

复制进去后，文件夹结构是这样的

![img](https://bbs.deepin.org/api/v1/thread/down_image?file_path=202011131402162433_thread_jag6w9WFbf6.png)

文件夹的名字不可更改，如果你解压出来的文件夹不是这个名字，那么改成这个。

然后在refind.conf文件的末尾添加下面这行

```
include themes/rEFInd-minimal/theme.conf
```

重启即可

特别提示，如果更改后无效，说明路径中的文件夹名称不对，认真检查即可。

至此就配置好了，尽情享用吧