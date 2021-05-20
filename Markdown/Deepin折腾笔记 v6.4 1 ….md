# Deepin折腾笔记 （重置版）v7.0.1

原作者： Yuchen Deng〔语晨〕「Deepin UOS 深度技术群：19346666」
二〇二〇年四月十六日
1本笔记所涉及到的代码或命令需结合上下文说明并理解，不能简单地复制粘贴后在终端执行。

现在基于原折腾笔记进行再度开发！



目录
第一章 Deepin 桌面配置与技巧 11
1.1 Super+S 切换工作区 . . . . . . . . . . . . . . . . . . . . . 11
1.2 善用强大的 Super 键 . . . . . . . . . . . . . . . . . . . . . 11
1.3 启动器搜索支持拼音 . . . . . . . . . . . . . . . . . . . . . . 11
1.4 “自然滚动”与 macOS、Win10 一致体验 . . . . . . . . . . . . . 11
1.5 加速软件更新 . . . . . . . . . . . . . . . . . . . . . . . . . 11
1.6 解决安装系统后更新失败 . . . . . . . . . . . . . . . . . . . . 11
1.7 预装系统安装应用商店 . . . . . . . . . . . . . . . . . . . . . 12
1.8 Chrome、VSCode 使用自定义标题栏 . . . . . . . . . . . . . . . 12
1.9 应用商店卸载软件失败 . . . . . . . . . . . . . . . . . . . . . 12
1.10 修改文件扩展名 . . . . . . . . . . . . . . . . . . . . . . . 12
1.11 删除不需要的文件打开方式 . . . . . . . . . . . . . . . . . . . 12
1.12 启动器隐藏不想看到的启动项 . . . . . . . . . . . . . . . . . . 12
1.13 创建数据盘 . . . . . . . . . . . . . . . . . . . . . . . . . 12
1.14 启动器创建“我的世界”启动项 . . . . . . . . . . . . . . . . . 13
1.15 VirtualBox 支持 USB2.0/3.0 设备 . . . . . . . . . . . . . 13
1.16 简易文字编辑器 . . . . . . . . . . . . . . . . . . . . . . . 13
1.17 调整桌面字体大小 . . . . . . . . . . . . . . . . . . . . . . 14
1.18 安装字体的另一种方法 . . . . . . . . . . . . . . . . . . . . 14
1.19 将当前位置加入书签 . . . . . . . . . . . . . . . . . . . . . 14
1.20 重置默认打开方式 . . . . . . . . . . . . . . . . . . . . . . 14
1.21 Nemo 文件管理器 . . . . . . . . . . . . . . . . . . . . . . 14
1.22 恢复默认文件管理器 . . . . . . . . . . . . . . . . . . . . . 14
1.23 VLC 视频播放器 . . . . . . . . . . . . . . . . . . . . . . . 14
1.24 audacious 音频播放器 . . . . . . . . . . . . . . . . . . . 15
第二章 Deepin 常见终端命令行 17
2.1 常用 Linux 文件目录命令 . . . . . . . . . . . . . . . . . . . 17
2.2 更换主机名 . . . . . . . . . . . . . . . . . . . . . . . . . 17
2.3 找到命令所在路径和所属软件包 . . . . . . . . . . . . . . . . . 17
2.4 APT 软件包管理扩展用法 . . . . . . . . . . . . . . . . . . . . 18
2.5 查询系统信息 . . . . . . . . . . . . . . . . . . . . . . . . . 18
2.6 tar 命令行压缩解压 . . . . . . . . . . . . . . . . . . . . . 18
2.7 7z 命令行压缩解压 . . . . . . . . . . . . . . . . . . . . . . 19
2.8 unar 万能解压 . . . . . . . . . . . . . . . . . . . . . . . . 19
2.9 查找删除重复文件 . . . . . . . . . . . . . . . . . . . . . . . 19
2.10 打印目录结构 . . . . . . . . . . . . . . . . . . . . . . . . 19
3
目录 目录
第三章 Deepin 硬件与驱动 21
3.1 安装 Nvidia 显卡私有驱动 . . . . . . . . . . . . . . . . . . 21
3.2 双显卡用户驱动 Nvidia 独显 . . . . . . . . . . . . . . . . . 21
3.3 更新官方 Nvidia 显卡驱动 . . . . . . . . . . . . . . . . . . 22
3.4 老 NVIDIA 显卡安装驱动 . . . . . . . . . . . . . . . . . . . 22
3.5 驱动显卡后黑屏或卡 LOGO . . . . . . . . . . . . . . . . . . . 22
3.6 双显卡驱动大黄蜂方案 . . . . . . . . . . . . . . . . . . . . . 22
3.7 显卡驱动与性能测试 . . . . . . . . . . . . . . . . . . . . . . 23
3.8 HP 打印机驱动 . . . . . . . . . . . . . . . . . . . . . . . . 23
3.9 HP 打印机备用驱动 . . . . . . . . . . . . . . . . . . . . . . 23
3.10 支持 Linux 的打印机 . . . . . . . . . . . . . . . . . . . . 23
3.11 触控版、无线网卡和蓝牙不正常 . . . . . . . . . . . . . . . . . 24
3.12 查询无线网卡型号 . . . . . . . . . . . . . . . . . . . . . . 24
3.13 无线网卡加速 . . . . . . . . . . . . . . . . . . . . . . . . 24
3.14 无线网卡解锁或蓝牙加锁 . . . . . . . . . . . . . . . . . . . 24
3.15 判断缺少哪些硬件驱动 . . . . . . . . . . . . . . . . . . . . 24
3.16 查询声卡信息 . . . . . . . . . . . . . . . . . . . . . . . . 24
第四章 Deepin 系统备份与还原 25
4.1 系统快照，折腾无忧 . . . . . . . . . . . . . . . . . . . . . . 25
4.2 硬盘或分区克隆及恢复 . . . . . . . . . . . . . . . . . . . . . 25
4.3 备份还原硬盘分区表 . . . . . . . . . . . . . . . . . . . . . . 25
4.4 再生龙启动盘制作 . . . . . . . . . . . . . . . . . . . . . . . 26
4.5 再生龙分区备份恢复到新硬盘 . . . . . . . . . . . . . . . . . . 26
4.6 再生龙备份恢复到大容量磁盘 . . . . . . . . . . . . . . . . . . 26
4.7 备份常见的用户配置 . . . . . . . . . . . . . . . . . . . . . . 27
4.8 备份还原硬盘 MBR . . . . . . . . . . . . . . . . . . . . . . 27
第五章 Deepin 系统维护与技巧 29
5.1 开机进入命令行 . . . . . . . . . . . . . . . . . . . . . . . . 29
5.2 主目录被误删除的恢复方法 . . . . . . . . . . . . . . . . . . . 29
5.3 解决与 Windows 时间不同步 . . . . . . . . . . . . . . . . . . 29
5.4 删除不需要的旧内核 . . . . . . . . . . . . . . . . . . . . . . 29
5.5 清除已卸载软件遗留配置 . . . . . . . . . . . . . . . . . . . . 29
5.6 假死后安全重启系统 . . . . . . . . . . . . . . . . . . . . . . 30
5.7 进程相关命令 . . . . . . . . . . . . . . . . . . . . . . . . . 30
5.8 查看与同步 GPT 分区 UUID . . . . . . . . . . . . . . . . . . 30
5.9 修改分区 UUID . . . . . . . . . . . . . . . . . . . . . . . . 30
5.10 sfdisk 创建磁盘 GPT 分区 . . . . . . . . . . . . . . . . . 30
5.11 修改磁盘卷标 . . . . . . . . . . . . . . . . . . . . . . . . 31
5.12 跨平台可读写文件系统 exfat 的格式化 . . . . . . . . . . . . . 31
5.13 修改系统运行级别 . . . . . . . . . . . . . . . . . . . . . . 31
5.14 离线安装软件 . . . . . . . . . . . . . . . . . . . . . . . . 32
Deepin UOS 深度技术群：19346666 4
目录 目录
5.15 升级操作系统内核 . . . . . . . . . . . . . . . . . . . . . . 33
5.16 自行编译内核 . . . . . . . . . . . . . . . . . . . . . . . . 33
5.17 重置所有用户配置 . . . . . . . . . . . . . . . . . . . . . . 33
5.18 终端 Ctrl+R 执行历史命令 . . . . . . . . . . . . . . . . . . 34
5.19 更换用户名及家目录 . . . . . . . . . . . . . . . . . . . . . 34
5.20 配置命令行默认 Python 版本 . . . . . . . . . . . . . . . . . 34
5.21 软件包管理技巧 . . . . . . . . . . . . . . . . . . . . . . . 34
5.21.1 禁止某软件包升级 . . . . . . . . . . . . . . . . . . . 34
5.21.2 允许某软件包升级 . . . . . . . . . . . . . . . . . . . 35
5.21.3 修正 dpkg -i *.deb 安装后缺少依赖 . . . . . . . . . . 35
5.21.4 强制清除 . . . . . . . . . . . . . . . . . . . . . . . 35
5.22 从源码编译安装软件包 . . . . . . . . . . . . . . . . . . . . 35
5.22.1 通过源码编译升级软件包 . . . . . . . . . . . . . . . . 35
5.22.2 基于源码编译 Shadowsocks-Qt5 . . . . . . . . . . . . 35
5.23 文件或目录权限管理 . . . . . . . . . . . . . . . . . . . . . 36
5.24 VirtualBox 虚拟机减肥 . . . . . . . . . . . . . . . . . . . 36
5.25 安装 TeXLive 最新版 . . . . . . . . . . . . . . . . . . . . 36
5.26 支持多架构：64 位系统安装 32 位软件 . . . . . . . . . . . . . 36
5.27 Backports 新版本软件安装 . . . . . . . . . . . . . . . . . . 36
5.28 Git 导出 Windows 行尾源码 . . . . . . . . . . . . . . . . . 37
5.29 架设 TFTP 服务器 . . . . . . . . . . . . . . . . . . . . . . 37
5.30 安装字体查看器 . . . . . . . . . . . . . . . . . . . . . . . 37
5.31 nmap 端口扫描 . . . . . . . . . . . . . . . . . . . . . . . 37
5.32 dns 和 arp 常用命令 . . . . . . . . . . . . . . . . . . . . 38
5.33 chroot 切换后访问网络 . . . . . . . . . . . . . . . . . . . 38
5.34 tty 文本模式连接 wifi . . . . . . . . . . . . . . . . . . . 38
5.35 调整 GPT 磁盘分区顺序 . . . . . . . . . . . . . . . . . . . 38
5.36 修改 SSH 端口号 . . . . . . . . . . . . . . . . . . . . . . 38
5.37 利用 ssh 登陆服务器 . . . . . . . . . . . . . . . . . . . . 38
5.38 利用 sshfs 挂载主机文件系统 . . . . . . . . . . . . . . . . . 39
5.39 scp 在服务器和本地间传送文件 . . . . . . . . . . . . . . . . 39
5.40 开机出现 Firmware Bug 日志 . . . . . . . . . . . . . . . . 39
5.41 ShadowSocks 代理上网 . . . . . . . . . . . . . . . . . . . 39
5.42 不重启切换终端与桌面 . . . . . . . . . . . . . . . . . . . . 39
5.43 查询系统服务 . . . . . . . . . . . . . . . . . . . . . . . . 40
5.44 查询服务依赖 . . . . . . . . . . . . . . . . . . . . . . . . 40
5.45 创建服务延时执行命令 . . . . . . . . . . . . . . . . . . . . 40
第六章 Deepin 办公与生产力 41
6.1 必备的 WPS 兼容字体包 . . . . . . . . . . . . . . . . . . . . 41
6.2 PDF 文件压缩 . . . . . . . . . . . . . . . . . . . . . . . . 41
6.3 卸载搜狗输入法，改用 Google 拼音 . . . . . . . . . . . . . . . 41
Deepin UOS 深度技术群：19346666 5
目录 目录
6.4 安装中州韵 fcitx-rime 输入法 . . . . . . . . . . . . . . . . 42
6.5 安装中州韵 rime-ibus 输入法 . . . . . . . . . . . . . . . . . 42
6.6 输入法无法开机自启动 . . . . . . . . . . . . . . . . . . . . . 43
6.7 解决中州韵偶尔无法输入中文 . . . . . . . . . . . . . . . . . . 43
6.8 搜狗输入法解决内存泄露 . . . . . . . . . . . . . . . . . . . . 43
6.9 Blender 视频剪辑多核渲染插件 . . . . . . . . . . . . . . . . . 43
6.10 Blender 视频剪辑多核渲染崩溃处置 . . . . . . . . . . . . . . 44
6.11 ffmpeg 音频视频编码 . . . . . . . . . . . . . . . . . . . . 44
6.11.1 ffmpeg 视频转换 . . . . . . . . . . . . . . . . . . . 44
6.11.2 批量编码转换 . . . . . . . . . . . . . . . . . . . . . 44
6.11.3 ffmpeg 视频连接 . . . . . . . . . . . . . . . . . . . 45
6.11.4 ffmpeg 提取音频 . . . . . . . . . . . . . . . . . . . 45
6.11.5 ffmpeg 视频混合音频 . . . . . . . . . . . . . . . . . 45
6.11.6 ffmpeg 视频合并音频 . . . . . . . . . . . . . . . . . 45
6.11.7 ffmpeg 截取视频 . . . . . . . . . . . . . . . . . . . 45
6.11.8 ffmpeg 指定时间合并 . . . . . . . . . . . . . . . . . 45
6.11.9 ffmpeg 调整播放速度 . . . . . . . . . . . . . . . . . 46
第七章 Deepin 启动与多系统 47
7.1 开机画面卡死卡桌面或者黑屏 . . . . . . . . . . . . . . . . . . 47
7.2 启动后桌面空白，任务栏消失 . . . . . . . . . . . . . . . . . . 47
7.3 系统启动分析 . . . . . . . . . . . . . . . . . . . . . . . . . 47
7.4 检查启动失败服务 . . . . . . . . . . . . . . . . . . . . . . . 47
7.5 查看开机日志 . . . . . . . . . . . . . . . . . . . . . . . . . 48
7.6 了解用户登陆情况 . . . . . . . . . . . . . . . . . . . . . . . 48
7.7 利用系统安装盘进 Live 模式 . . . . . . . . . . . . . . . . . . 48
7.8 Live 模式修复 GRUB 引导 . . . . . . . . . . . . . . . . . . . 48
7.9 GRUB 维护技巧 . . . . . . . . . . . . . . . . . . . . . . . . 49
7.9.1 设置默认系统为用户选择 . . . . . . . . . . . . . . . . . 49
7.9.2 隐藏启动菜单 . . . . . . . . . . . . . . . . . . . . . 49
7.10 禁止 GRUB 检测其它系统 . . . . . . . . . . . . . . . . . . . 49
7.11 屏蔽开关机屏幕日志 . . . . . . . . . . . . . . . . . . . . . 49
7.12 开机关机巨大 LOGO . . . . . . . . . . . . . . . . . . . . . 50
7.13 修正启动或关机界面分辨率 . . . . . . . . . . . . . . . . . . . 50
7.14 Ventoy 制作多系统启动盘 . . . . . . . . . . . . . . . . . . 50
7.15 Win10 USB 启动盘制作 . . . . . . . . . . . . . . . . . . . 50
7.16 安装 Deepin 与 Windows 双系统 . . . . . . . . . . . . . . . 51
7.17 双系统修复 Windows EFI . . . . . . . . . . . . . . . . . . 51
7.18 Windows 系统读写 EFI 分区 . . . . . . . . . . . . . . . . . 51
7.19 制作 USB 启动盘 . . . . . . . . . . . . . . . . . . . . . . 51
7.20 EFI 引导分区不要删除 ubuntu . . . . . . . . . . . . . . . . 52
7.21 误删 EFI 分区后的还原 . . . . . . . . . . . . . . . . . . . 52
Deepin UOS 深度技术群：19346666 6
目录 目录
7.22 恢复 Deepin 引导主题 . . . . . . . . . . . . . . . . . . . . 52
7.23 命令行查看 EFI 启动项 . . . . . . . . . . . . . . . . . . . 52
7.24 查看当前 EFI 启动项详情 . . . . . . . . . . . . . . . . . . . 53
7.25 删除重复的 EFI 启动项 . . . . . . . . . . . . . . . . . . . 53
7.26 调整 EFI 启动项顺序 . . . . . . . . . . . . . . . . . . . . 53
7.27 创建 EFI 启动项 . . . . . . . . . . . . . . . . . . . . . . 53
7.28 删除 EFI 启动项 . . . . . . . . . . . . . . . . . . . . . . 53
7.29 查看硬盘分区信息 . . . . . . . . . . . . . . . . . . . . . . 53
7.30 修复黑苹果 Clover 引导 . . . . . . . . . . . . . . . . . . . 53
7.31 Live 模式调整磁盘分区大小 . . . . . . . . . . . . . . . . . . 54
7.32 Live 模式防锁屏后无法登陆 . . . . . . . . . . . . . . . . . . 54
7.33 解决多系统启动缓慢 . . . . . . . . . . . . . . . . . . . . . 54
7.34 VirtualBox 从 U 盘启动 . . . . . . . . . . . . . . . . . . 54
第八章 Deepin 远程控制与共享 55
8.1 向日葵远程控制 . . . . . . . . . . . . . . . . . . . . . . . . 55
8.2 TeamViewer 远程控制 . . . . . . . . . . . . . . . . . . . . 55
8.3 AnyDesk 远程控制 . . . . . . . . . . . . . . . . . . . . . . 55
8.3.1 提高 AnyDesk 远程控制权限 . . . . . . . . . . . . . . . 55
8.3.2 AnyDesk 自动连接控制 . . . . . . . . . . . . . . . . . 55
8.3.3 禁止 AnyDesk 自启动 . . . . . . . . . . . . . . . . . 55
8.4 VNC 远程控制 . . . . . . . . . . . . . . . . . . . . . . . . 55
8.5 RDP 协议连接 Windows 远程桌面 . . . . . . . . . . . . . . . . 56
8.6 Linux 打印机共享 . . . . . . . . . . . . . . . . . . . . . . 56
8.7 Windows 打印机共享 . . . . . . . . . . . . . . . . . . . . . 56
8.8 Windows 云打印共享 . . . . . . . . . . . . . . . . . . . . . 56
第九章 Deepin 运行 Windows 软件 57
9.1 安装运行 Windows 绿色软件 . . . . . . . . . . . . . . . . . . 57
9.2 为大型 Windows 软件创建独立运行环境 . . . . . . . . . . . . . 57
9.3 修改 QQ 聊天窗口文字大小 . . . . . . . . . . . . . . . . . . . 57
9.4 双击运行 Windows 软件 . . . . . . . . . . . . . . . . . . . . 57
9.5 适配绿色版 Photoshop CC . . . . . . . . . . . . . . . . . . 58
9.6 卸载 Windows 软件 . . . . . . . . . . . . . . . . . . . . . 58
第十章 Deepin 疑难问题解答 59
10.1 安装 Deepin 时找不到 M.2 硬盘 . . . . . . . . . . . . . . . 59
10.2 应用程序假死或无响应 . . . . . . . . . . . . . . . . . . . . 59
10.3 禁用 IPv6 解决 QQ 图片显示 . . . . . . . . . . . . . . . . . 59
10.4 从 3D 游戏返回后屏幕闪烁 . . . . . . . . . . . . . . . . . . 59
10.5 关闭错误报警蜂鸣声 . . . . . . . . . . . . . . . . . . . . . 60
10.6 睡眠/休眠唤醒之后触摸板失灵 . . . . . . . . . . . . . . . . . 60
10.7 任务栏/启动器消失 . . . . . . . . . . . . . . . . . . . . . . 61
Deepin UOS 深度技术群：19346666 7
目录 目录
10.8 窗口无响应或系统卡顿 . . . . . . . . . . . . . . . . . . . . 61
10.9 创建 DEB 安装包 . . . . . . . . . . . . . . . . . . . . . . 61
第十一章 Deepin 终端操作技巧集锦 63
11.1 以管理员身份自启动 . . . . . . . . . . . . . . . . . . . . . 63
11.2 递归更改文件所有者 . . . . . . . . . . . . . . . . . . . . . 63
11.3 从指定类型文件中查找 . . . . . . . . . . . . . . . . . . . . 63
11.4 更好的搜索方法 . . . . . . . . . . . . . . . . . . . . . . . 63
11.5 将行末多个空行转换成一个空行 . . . . . . . . . . . . . . . . . 63
11.6 ls 只显示目录名 . . . . . . . . . . . . . . . . . . . . . . 63
11.7 ls 只显示文件 . . . . . . . . . . . . . . . . . . . . . . . 63
11.8 ls 显示软链接 . . . . . . . . . . . . . . . . . . . . . . . 64
11.9 为子目录和文件设置不同权限 . . . . . . . . . . . . . . . . . . 64
11.10 为指定类型文件设置可执行权限 . . . . . . . . . . . . . . . . 64
11.11 获取脚本文件所在路径 . . . . . . . . . . . . . . . . . . . . 64
11.12 批量文本替换 . . . . . . . . . . . . . . . . . . . . . . . 64
11.13 获取 CPU 个数并四则运算后导出环境变量 . . . . . . . . . . . . 64
11.14 命令行解压缩到指定目录 . . . . . . . . . . . . . . . . . . . 64
11.15 通过 git 实现跨平台的 grep 用法 . . . . . . . . . . . . . . 65
11.16 打印当前目录路径 . . . . . . . . . . . . . . . . . . . . . . 65
11.17 初始化当前用户配置 . . . . . . . . . . . . . . . . . . . . . 65
11.18 初始化 root 用户配置 . . . . . . . . . . . . . . . . . . . 65
11.19 查询命令软链接 . . . . . . . . . . . . . . . . . . . . . . . 65
11.20 top 命令技巧 . . . . . . . . . . . . . . . . . . . . . . . 65
11.21 查看指定行的内容 . . . . . . . . . . . . . . . . . . . . . . 65
11.22 搜索匹配多个关键词 . . . . . . . . . . . . . . . . . . . . . 66
11.23 字符串截取 . . . . . . . . . . . . . . . . . . . . . . . . 66
第十二章 ArchLinux DDE 折腾笔记 67
12.1 下载 Arch 安装镜像，阅读安装指南 . . . . . . . . . . . . . . 67
12.2 安装 1：连接网络 . . . . . . . . . . . . . . . . . . . . . . 67
12.3 安装 2：分区与挂载 . . . . . . . . . . . . . . . . . . . . . 67
12.4 安装 3：换国内源 . . . . . . . . . . . . . . . . . . . . . . 67
12.5 安装 4：安装与配置 . . . . . . . . . . . . . . . . . . . . . 68
12.6 安装 5：后期批处理 . . . . . . . . . . . . . . . . . . . . . 68
12.7 使用 LTS 内核提高稳定性 . . . . . . . . . . . . . . . . . . . 69
12.8 为 LTS 内核安装 dkms 后缀包 . . . . . . . . . . . . . . . . 70
12.9 安装 NVIDIA 显卡驱动 . . . . . . . . . . . . . . . . . . . . 70
12.10 更多软件安装 . . . . . . . . . . . . . . . . . . . . . . . 70
12.11 pacman 常见用法 . . . . . . . . . . . . . . . . . . . . . 70
12.12 清除孤儿包 . . . . . . . . . . . . . . . . . . . . . . . . 71
12.13 yay 替代 pacman . . . . . . . . . . . . . . . . . . . . . 71
12.14 yay 扩展用法 . . . . . . . . . . . . . . . . . . . . . . . 71
Deepin UOS 深度技术群：19346666 8
目录 目录
12.15 yay 缓存路径 . . . . . . . . . . . . . . . . . . . . . . . 71
12.16 免密码挂载分区 . . . . . . . . . . . . . . . . . . . . . . . 71
12.17 备用 Nemo 文件管理器 . . . . . . . . . . . . . . . . . . . 72
12.18 KWin 无法开启窗口特效 . . . . . . . . . . . . . . . . . . . 72
12.19 外部磁盘挂载改/media/$USER . . . . . . . . . . . . . . . . 72
12.20 删除不再需要的软件 . . . . . . . . . . . . . . . . . . . . . 72
12.21 禁止无密码授权 . . . . . . . . . . . . . . . . . . . . . . . 72
12.22 禁止 root 用户登陆 . . . . . . . . . . . . . . . . . . . . 72
第十三章 Debian 10 折腾笔记 73
13.1 自定义安装 GNOME 桌面 . . . . . . . . . . . . . . . . . . . 73
13.2 Debian Shell 连接 wifi . . . . . . . . . . . . . . . . . . 73
13.3 更换国内软件源 . . . . . . . . . . . . . . . . . . . . . . . 73
13.4 终端命令自动完成 . . . . . . . . . . . . . . . . . . . . . . 74
13.5 驱动无线网卡 . . . . . . . . . . . . . . . . . . . . . . . . 74
13.6 驱动 Nvidia 显卡 . . . . . . . . . . . . . . . . . . . . . 74
13.7 安装中州韵 rime-ibus 输入法 . . . . . . . . . . . . . . . . 74
13.8 为终端设置 Ctrl+Alt+T 快捷键 . . . . . . . . . . . . . . . . 74
13.9 启用触摸板轻拍以点击 . . . . . . . . . . . . . . . . . . . . 74
13.10 启用触摸板双指滚动 . . . . . . . . . . . . . . . . . . . . . 74
13.11 重启 GNOME Shell . . . . . . . . . . . . . . . . . . . . . 75
13.12 启用 macOS 风格桌面 . . . . . . . . . . . . . . . . . . . . 75
13.13 启用 Windows 风格桌面 . . . . . . . . . . . . . . . . . . . 75
13.14 NetworkManager 托管网络 . . . . . . . . . . . . . . . . . 75
13.15 显示托盘图标 . . . . . . . . . . . . . . . . . . . . . . . 75
13.16 免密码挂载分区 . . . . . . . . . . . . . . . . . . . . . . . 75
13.17 Backport 软件安装 . . . . . . . . . . . . . . . . . . . . 75
13.18 Debian 急救模式修复 GRUB 引导 . . . . . . . . . . . . . . . 76
第十四章 Ubuntu 18.04 LTS 折腾笔记 77
14.1 Ubuntu 最小化安装 . . . . . . . . . . . . . . . . . . . . . 77
14.2 更换国内软件源 . . . . . . . . . . . . . . . . . . . . . . . 77
14.3 驱动独立显卡 . . . . . . . . . . . . . . . . . . . . . . . . 77
14.4 禁用 GNOME 软件的 Snap 插件 . . . . . . . . . . . . . . . . 77
14.5 安装优化程序 . . . . . . . . . . . . . . . . . . . . . . . . 77
14.6 界面设置与优化 . . . . . . . . . . . . . . . . . . . . . . . 77
14.7 添加五笔输入法 . . . . . . . . . . . . . . . . . . . . . . . 78
14.8 添加与卸载 PPA 源 . . . . . . . . . . . . . . . . . . . . . 78
第十五章 更多笔记·部分已过时 79
15.1 LightDM 配置维护 . . . . . . . . . . . . . . . . . . . . . 79
15.1.1 修改 lightdm 登陆分辨率 . . . . . . . . . . . . . . . 79
15.1.2 解决 lightdm 不加载.profile . . . . . . . . . . . . 79
Deepin UOS 深度技术群：19346666 9
目录 目录
15.1.3 lightdm 用户自动登陆 . . . . . . . . . . . . . . . . 79
15.2 屏幕亮度修正 . . . . . . . . . . . . . . . . . . . . . . . . 79
15.2.1 方法一 . . . . . . . . . . . . . . . . . . . . . . . . 79
15.2.2 方法二 . . . . . . . . . . . . . . . . . . . . . . . . 80
15.3 创建 Android 可连接的 WIFI 热点 . . . . . . . . . . . . . . 80
15.4 Wine 配置方法 . . . . . . . . . . . . . . . . . . . . . . . 81
15.4.1 配置 Wine 纯净版 . . . . . . . . . . . . . . . . . . 81
15.4.2 彻底清理 Wine . . . . . . . . . . . . . . . . . . . . 81
15.4.3 Wine 调用批处理时字体错误处理 . . . . . . . . . . . . . 81
15.4.4 64 位系统，通过 Wine 模拟纯 32 位 Windows . . . . . . 82
15.4.5 英文系统安装 Wine 及中文支持 . . . . . . . . . . . . . 82
15.5 MlDonkey 选项设置 . . . . . . . . . . . . . . . . . . . . . 82
Deepin UOS 深度技术群：19346666 10
第一章 Deepin 桌面配置与技巧
1.1 Super+S 切换工作区
1 Super键就是WIN键。
2 这个工作区快捷切换键最初由Ubuntu发行版引入。
3 目前Deepin只能简单的将多个工作区放在一行横向排列。
4 缺少智能的多行自适应布局。
1.2 善用强大的 Super 键
1 Super ：启动器
2 Super+S ：显示工作区
3 Super+W ：显示当前工作区的窗口
4 Super+A ：显示所有工作区的窗口
5 Super+D ：显示桌面
6 Super+E ：文件管理器
7 Super+L ：锁屏
1.3 启动器搜索支持拼音
1 开始菜单或启动器键盘输入“xk”，将显示“显卡驱动管理器”，支持模糊匹配。
2 简拼、全拼都可以。
1.4 “自然滚动”与 macOS、Win10 一致体验
1 控制中心-鼠标：打开“自然滚动”选项，可实现笔记本电脑触控板双指上下滚动页面时与手机、
平板、macOS、Win10 保持相同体验。
1.5 加速软件更新
1 控制中心-更新-更新设置，取消“智能软件源”，并切换到“中国科学技术大学”镜像源。
1.6 解决安装系统后更新失败
1 通过“控制中心”更新时，如果提示“更新失败”，则可以按下快捷键Ctrl+Alt+T，在弹出的
终端中输入命令：
2 sudo apt upgrade
3 回车后按提示操作即可。
4 技巧推荐：输入命令的过程中按一次Tab键补全，两次Tab键候选。
11
1.7 预装系统安装应用商店 第一章 DEEPIN 桌面配置与技巧
1.7 预装系统安装应用商店
1 默认预装Deepin专业版的品牌笔记本没有集成应用商店，Deepin官方给出了解决方案：
2 https://mp.weixin.qq.com/s/UGX22z_jTZ2BN0BXV54hBw
3 也可以更新系统后选择在命令行安装，按下快捷键Ctrl+Alt+T，在弹出的终端中输入命令：
4 sudo apt install deepin-appstore
5 按提示操作安装完成后，按下Super键（WIN键），就可以找到“应用商店”图标了。
1.8 Chrome、VSCode 使用自定义标题栏
1 系统原生标题栏很难看，和Chrome和VSCode自身的风格非常不协调。
2 Google Chrome浏览器可以在标题栏右键，去掉“使用系统标题栏和边框”。
3 VSCode可以在“文件-首选项-设置-窗口-Title Bar Style”中选择“custom”。
4 这样就美观多了。
1.9 应用商店卸载软件失败
1 Ctrl+Alt+T打开终端，输入命令：sudo apt install -f
2 回车执行后重新在应用商店卸载即可。
1.10 修改文件扩展名
1 方法一：在要修改的文件上弹出右键菜单，“属性”窗口可完成文件名、扩展名修改。
2 方法二：进入文件所在目录，右键“在终端中打开”，执行：mv filename.txt filename.
sh
1.11 删除不需要的文件打开方式
1 文件管理器进入主目录，Ctrl+H显示隐藏文件，进入.confg目录，编辑mimeapps.list。
1.12 启动器隐藏不想看到的启动项
1 文件管理器打开系统盘，进入/usr/share目录，在applications目录上右键“以管理员身份
打开”。在不想看到的启动项图标上右键，“打开方式”选择“编辑器”，添加：
NoDisplay=true
2 保存。
1.13 创建数据盘
1 只要存在一个不挂载任何路径的分区，且该分区的卷标为“_dde_data”即可。卷标修改请参考
“修改磁盘卷标”小节。
Deepin UOS 深度技术群：19346666 12
第一章 DEEPIN 桌面配置与技巧 1.14 启动器创建“我的世界”启动项
1.14 启动器创建“我的世界”启动项
1 在应用商店里安装软件后，就可以在启动器里找到该软件的一个启动项，启动软件变得非常方
便。在启动项右键菜单上还提供了“发送到桌面”、“发送到任务栏”、“开机自动启动”
等简捷功能。
2 而所谓的启动项，本质就是一个后缀为“.desktop”的文件，可以在系统盘/usr/share/
applications/里看到。
3 但是，在/usr/share/applications/里创建启动项并不是最佳的位置。
4 最佳位置在主目录 ~/.local/share/applications 里。
5 下面以创建Minecraft(我的世界)为例讲解。
6 首先用编辑器创建文件 ~/.local/share/applications/Minecraft.desktop ,添加以下
内容：
7 [Desktop Entry]
8 Categories=Game;
9 Comment=Minecraft
10 Exec=/home/<用户名>/Minecraft/Minecraft.sh
11 Icon=minecraft
12 Name=Minecraft
13 Name[zh_CN]=我的世界
14 Terminal=false
15 Type=Application
16 X-Deepin-Vendor=user-custom
17 特别注意1：所有的路径都必须是绝对路径，而且不识别$HOME、~这些常见的bash变量。
18 特别注意2：Icon虽然可以用绝对路径的图标，但不能自适应大小。推荐把图标拷贝到~/.local
/share/icons/hicolor/的各个尺寸目录里，文件名为minecraft。
19 Minecraft.sh就是我的世界的启动脚本，内容如下：
20 #!/bin/bash
21 cd $HOME/Zz/Minecraft
22 java -jar HMCL.jar
23 HMCL启动器下载地址：https://github.com/huanghongxun/HMCL
24 需要安装Java运行时：sudo apt install default-jre openjfx
1.15 VirtualBox 支持 USB2.0/3.0 设备
1 首先要安装扩展：sudo apt install virtualbox-extension-pack
2 其次要添加用户组：sudo adduser <用户名> vboxusers
3 重启生效。
4 查看确认用户组：groups <用户名>
5 从用户组中删除：sudo deluser <用户名> vboxusers
1.16 简易文字编辑器
1 deepin的编辑器打开大文件太慢了，这个问题官方有bug报告，说是为了兼容触屏而选择的一种
妥协方案，结果牺牲了打开大文件时的性能。
2 暂时的解决：考虑安装leafpad，用于打开大的文本文件。
3 sudo apt install leafpad #简易文字编辑器
Deepin UOS 深度技术群：19346666 13
1.17 调整桌面字体大小 第一章 DEEPIN 桌面配置与技巧
1.17 调整桌面字体大小
1 控制中心 - 个性化 - 字体，将大小调整为15。
1.18 安装字体的另一种方法
1 Deepin提供了字体安装器，拖动字体文件到这个应用上就完成字体安装了，很方便。
2 但有时为了在不同Deepin系统里使用相同的字体，还有一个方法是把ttf字体文件拷贝到$HOME
/.local/share/fonts目录下。
3 平常注意这个目录的备份，在新系统上还原配置，就可以享受相同的字体了。
1.19 将当前位置加入书签
1 文件管理器打开常用目录，按下快捷键Ctrl+D，可加入左侧书签，方便以后快速打开。
1.20 重置默认打开方式
1 部分四字母后缀名的文件无法设置默认打开方式，估计是BUG。例如xlsx电子表格文件，默认总
是用归档管理器file-roller打开。
2 解决方法：删除默认打开方式配置文件～/.config/mimeapps.list，注销。
1.21 Nemo 文件管理器
1 深度文件管理器在处理大量图片时，容易崩溃。此外，删除存在大量文件的目录时，会很低效且
偶尔删除失败。
2 推荐安装Nemo文件管理器作为备用。
3 sudo apt install nemo gnome-terminal
4 安装完成后，启动器中寻找“文件”。
1.22 恢复默认文件管理器
1 安装Visual Studio Code后，会发现在谷歌浏览器中下载文件后，如果点击“在文件夹中显
示”时弹出Visual Studio Code窗口。
2 解决办法：在文件管理器里随意创建一个空文件夹，然后在这个文件夹上点击右键，从右键菜单
里选择“打开方式”，把“文件管理器”设置为默认程序即可。
3 此外，控制中心有常用的默认程序配置功能。
1.23 VLC 视频播放器
1 作为深度自带的视频播放器的补充，推荐安装跨平台的视频播放器VLC作为备用。
2 优点是速度快，兼容所有视频格式。
3 sudo apt install vlc
Deepin UOS 深度技术群：19346666 14
第一章 DEEPIN 桌面配置与技巧 1.24 AUDACIOUS 音频播放器
1.24 audacious 音频播放器
1 深度自带的音频播放器默认单曲循环，没有单曲播放后自行停止的功能。
2 而audacious号称Linux系统下的Foobar2000，值得推荐！
3 sudo apt install audacious
Deepin UOS 深度技术群：19346666 15
1.24 AUDACIOUS 音频播放器 第一章 DEEPIN 桌面配置与技巧
Deepin UOS 深度技术群：19346666 16
第二章 Deepin 常见终端命令行
2.1 常用 Linux 文件目录命令
1 ls #列出目录
2 ls -l #使用格式化列出文件
3 ls -al #使用格式化列出所有文件，含隐藏文件
4 cd dir #进入目录dir
5 cd #进入主目录home
6 pwd #显示当前目录
7 mkdir dir #创建目录dir
8 rm file #删除文件file
9 rm -r dir #删除目录dir及子目录
10 rm -f file #强制删除文件file
11 rm -rf dir #强制删除目录dir及子目录
12 cp file1 file2 #将文件file1复制到文件file2
13 cp -r dir1 dir2 #将目录dir1复制到目录dir2
14 mv file1 file2 #将file1重命名或移动到file2
15 ln -s file link #创建file的符号连接link
16 touch file #创建file
17 cat file #显示file内容
18 more file #分屏查看file的内容
19 less file #滚动查看file的内容
20 head file #查看file的前10行
21 tail file #查看file的后10行
22 tree /boot/efi #查看目录树结构，需要安装：sudo apt install tree
2.2 更换主机名
1 sudo deepin-editor /etc/hostname
2 替换成新的主机名，重启电脑。
2.3 找到命令所在路径和所属软件包
1 查找编辑器所在路径：which deepin-editor
2 输出“/usr/bin/deepin-editor”
3 查询文件属于哪个包：dpkg -S /usr/bin/deepin-editor
4 输出“deepin-editor: /usr/bin/deepin-editor”
5 冒号之前的“deepin-editor”就是软件包。
17
2.4 APT 软件包管理扩展用法 第二章 DEEPIN 常见终端命令行
2.4 APT 软件包管理扩展用法
1 大多数的软件安装、卸载都应该在深度系统“应用商店”里可视化操作。下面以软件包“
package-name”为例，总结软件包相关的常用命令：
2 安装软件包：sudo apt install package-name
3 安装并修复依赖关系：sudo apt install -f package-name
4 重新安装软件包：sudo apt install --reinstall package-name
5 移除软件包但保留系统配置：sudo apt remove package-name
6 移除软件包且清除系统配置：sudo apt purge package-name
7 移除不需要的软件包并清除配置：sudo apt autoremove --purge
8 罗列所有软件包：apt list *weixin*
9 罗列已安装软件包：apt list --installed fcitx*
10 搜索软件包：apt search --names-only package-name
11 查看软件包内文件明细：dpkg -L package-name
2.5 查询系统信息
1 安装查询软件：sudo apt install neofetch screenfetch
2 终端查询命令：neofetch 或 screenfetch
3 常用命令还有：
4 uname -a #查询内核版本
5 cat /proc/cpuinfo #查询CPU信息
6 hostname #查看计算机名
7 lspci #列出所有PCI设备
8 lsusb #列出所有USB设备
9 lsmod #列出加载的内核模块
10 env #查看环境变量资源
11 free -m #查看内存使用量和交换区使用量
12 df -h #查看各分区使用情况
13 ifconfig #查看网络接口属性，需 sudo apt install net-tools 或 ip address
14 route -n #查看路由表，或 ip route
2.6 tar 命令行压缩解压
1 压缩： tar -cJvf [目标文件名].tar.xz [源文件名/目录名]
2 解压： tar -xJvf [源文件名].tar.xz
3 -c: 建立压缩档案
4 -x：解压
5 -t：查看内容
6 -r：向压缩归档文件末尾追加文件
7 -u：更新原压缩包中的文件
8 -v：显示所有过程
9 -J：有LZMA属性的
10 -z：有gzip属性的
11 -j：有bz2属性的
12 万能解压：tar -xvf filename，可根据文件后缀名自动判断。
Deepin UOS 深度技术群：19346666 18
第二章 DEEPIN 常见终端命令行 2.7 7Z 命令行压缩解压
2.7 7z 命令行压缩解压
1 软件安装：sudo apt install p7zip-full
2 压缩： 7z a [目标文件名].7z [源文件名/目录名]
3 解压并解包： 7z x [源文件名].7z
2.8 unar 万能解压
1 unar对压缩包中的中文编码支持非常好，是一个近乎万能的解压工具，用法很简单：
2 用法：unar [options] archive [files ...]
3 帮助：unar --help
2.9 查找删除重复文件
1 首先安装命令行工具：sudo apt install fdupes
2 查找重复文件：使用-r选项在每个目录包括其子目录中递归搜索重复文件。
3 删除重复文件：使用-d选项删除重复文件，同时由用户选择保留一个副本。
4 只保留第一个：使用-dN选项删除重复文件，同时只保留第一个副本。慎用！
5 查找当前目录及子目录重复文件：fdupes -r .
6 删除当前目录重复文件：fdupes -d .
7 删除当前目录及子目录重复文件且只保留第一个副本：fdupes -rdN .
2.10 打印目录结构
1 安装：sudo apt install tree
2 例如：tree /boot/efi/EFI
Deepin UOS 深度技术群：19346666 19
2.10 打印目录结构 第二章 DEEPIN 常见终端命令行
Deepin UOS 深度技术群：19346666 20
第三章 Deepin 硬件与驱动
3.1 安装 Nvidia 显卡私有驱动
1 开始菜单或启动器键盘输入“xk”搜索“显卡驱动管理器”并启动，即可安装显卡驱动。如果显
卡驱动管理器安装失败，请继续往下看。
2 首先判断是单显卡，还是双显卡：lspci |grep -Ei "VGA|3D|NVIDIA"
3 确定Intel和Nvidia双显卡后，请参考第二节“双显卡用户驱动N卡独显”。
4 否则请检测适合本机的显卡驱动：nvidia-detect
5 如果提示nvidia-detect命令不存在，则先安装：sudo apt install nvidia-detect
6 如果检测结果返回nvidia-driver，则：sudo apt install nvidia-driver
7 如果仍然失败，则尝试彻底禁掉nouveau驱动：sudo dedit /etc/default/grub
8 修改：GRUB_CMDLINE_LINUX="rd.driver.blacklist=nouveau modprobe.blacklist
=nouveau nvidia-drm.modeset=1"
9 保存退出后执行：sudo update-grub
10 重启电脑，再次执行 sudo apt install nvidia-driver 后重启。
11 如果仍然失败，请参考第三节“更新官方Nvidia显卡驱动”内容。
3.2 双显卡用户驱动 Nvidia 独显
1 第一步：xrandr --listproviders #双显卡应该有两行输出，但也可能该命令无法识别
2 第二步：确定Nvidia显卡的BusID，执行lspci |grep NVIDIA
3 示例输出：04:00.0 3D controller: NVIDIA Corporation GK208M [GeForce 920M]
4 根据行首数字“04:00.0”确定显卡的BusID为："PCI:4:0:0"。
5 第三步：编写Nvidia显卡的配置文件，sudo dedit /etc/X11/xorg.conf，复制以下内容
后替换你显卡的BusID。注意：以下步骤如果有一个字母错误，都可能启动黑屏。
6 Section "Module"
7 Load "modesetting"
8 EndSection
9 Section "Device"
10 Identifier "nvidia"
11 Driver "nvidia"
12 BusID "PCI:4:0:0"
13 EndSection
14 第四步：在LightDM启动时设置独显运算核显输出
15 参考以下内容修改配置：sudo dedit /etc/lightdm/lightdm.conf
16 [Seat:*]
17 ...
18 display-setup-script=sh -c "xrandr --setprovideroutputsource
modesetting NVIDIA-0; xrandr --auto"
19 第五步：安装Nvidia显卡驱动和工具 sudo apt install nvidia-driver nvidia-smi
nvidia-settings
20 重启后，lspci -k |grep -A 2 -E "VGA|3D" 或者nvidia-smi判断N卡驱动情况。
21 改编优化自：一本正经的胡说八道（QQ：1534646530）
21
3.3 更新官方 NVIDIA 显卡驱动 第三章 DEEPIN 硬件与驱动
3.3 更新官方 Nvidia 显卡驱动
1 驱动下载：https://www.nvidia.cn/drivers/unix/
2 首先进入系统运行级别3：
3 sudo init 3
4 登陆shell，如果曾经安装过N卡驱动，则需要先卸载旧Nvidia驱动：
5 sudo apt purge nvidia*
6 sudo apt autoremove --purge
7 然而就可以顺利安装从英伟达官方网站下载的最新驱动了：
8 sudo ./NVIDIA-Linux-x86_64-430.34.run
9 安装完成后如果重启黑屏，请参看疑难解答双显卡相关内容。
10 安装前需要右键属性添加可执行权限，或者：
11 sudo chmod +x ./NVIDIA-Linux-x86_64-430.34.run
12 重启后可命令行查看硬件驱动情况：lspci -k |grep -A 2 -E "VGA|3D"
13 还可以：sudo apt install nvidia-smi，之后执行nvidia-smi命令查询。
3.4 老 NVIDIA 显卡安装驱动
1 首先安装N卡驱动检测工具：sudo apt install nvidia-detect
2 运行检测命令：nvidia-detect
3 输出示例：
4 Detected NVIDIA GPUs:...
5 It is recommended to install the
6 nvidia-legacy-340xx-driver
7 根据提示安装驱动：sudo apt install nvidia-legacy-340xx-driver
8 详见：https://wiki.deepin.org/wiki/%E6%98%BE%E5%8D%A1
3.5 驱动显卡后黑屏或卡 LOGO
1 Ctrl+Alt+F2进tty2，sudo apt purge nvidia*卸载N卡驱动后，按上面双显卡步骤操作。
2 如果xrandr --listproviders显示只有独显，请省略双显卡驱动的第四步。
3.6 双显卡驱动大黄蜂方案
1 参考：https://wiki.archlinux.org/index.php/Bumblebee_(%E7%AE%80%E4%BD
%93%E4%B8%AD%E6%96%87)
2 NVIDIA的Optimus技术， 允许自动切换显卡的使用，权衡了续航和性能之间的问题。
3 大黄蜂"Bumblebee 致力于使 NVIDIA Optimus 在 GNU/Linux 系统上可用，实现两块不同
的供电配置的显卡同时插入使用，共享同一个 framebuffer。"
4 Bumblebee 试图模拟 Optimus 技术的行为；当需要的时候，使用独立显卡进行渲染，不使用
的时候则关闭。
5 查询是否可用：optirun glxgears -info
6 强制独显输出：optirun command...
7 奇怪的是：vblank_mode=0 optirun glxgears 帧频很低，原因未知。
Deepin UOS 深度技术群：19346666 22
第三章 DEEPIN 硬件与驱动 3.7 显卡驱动与性能测试
3.7 显卡驱动与性能测试
1 可以通过在终端执行FPS测试命令，判断自己显卡驱动是否正常工作：
2 sudo apt install mesa-utils
3 vblank_mode=0 glxgears
4 一般FPS能达到3000以上，就说明显卡驱动能正常工作了。
5 建议使用应用商店的“显卡驱动管理器”切换或者安装驱动。
6 不到迫不得已，请不要升级内核。
7 官方维基：https://wiki.deepin.org/index.php?title=%E6%98%BE%E5%8D%A1&
language=en#.E7.AE.80.E4.BB.8B
8 NVIDIA显卡安装闭源驱动后，vblank_mode=0选项无效，需要从自带的配置程序“OpenGL
Settings”中取消垂直同步刷新功能。
9 sudo apt install nvidia-settings
10 nvidia-settings
3.8 HP 打印机驱动
1 推荐在“打印管理器”或“打印设置”中添加打印机。也可以自行安装：
2 sudo apt install hplip hplip-gui hplip-plugin
3 安装完成后，终端运行命令：hp-setup，按步骤添加打印机。
4 Linux系统上安装的打印机目前还不知道如何和Windows系统用户共享。
5 同为Deepin系统的话，“打印设置”里添加网络打印机可以轻松共享。
3.9 HP 打印机备用驱动
1 foo2zjs是一个基于ZjStream协议的Linux开源驱动，项目地址：http://foo2zjs.rkkda.
com
2 源码下载地址：http://foo2zjs.rkkda.com/foo2zjs.tar.gz
3 可以通过项目地址查到支持的打印机列表。对于不支持的打印机，作者还提供了更多驱动，搜索
“Unsupported Printer”即可在表格中定位。
4 一定要认真按照作者提示：不要从仓库中下载，而是选择从源码中编译安装。
5 编译：make
6 安装：sudo make install
7 之后即可通过启动器“打印设置”添加打印机。
8 更多打印机驱动：http://rkkda.com/
3.10 支持 Linux 的打印机
1 Brother：https://www.brother.cn/
2 奔图：http://www.pantum.com/
3 以上品牌部分打印机官方提供驱动，未经测试，仅供参考。
Deepin UOS 深度技术群：19346666 23
3.11 触控版、无线网卡和蓝牙不正常 第三章 DEEPIN 硬件与驱动
3.11 触控版、无线网卡和蓝牙不正常
1 作者：Sam（QQ：13976001016）
2 更新硬件驱动：linux-firmware
3 可以从这里下载Ubuntu的硬件驱动最新版：http://ftp.sjtu.edu.cn/ubuntu/pool/
main/l/linux-firmware/
4 例如当前最新版：http://ftp.sjtu.edu.cn/ubuntu/pool/main/l/linux-firmware/
linux-firmware_1.186_all.deb
5 下载安装，重启。
6 如果问题仍然无法解决，请尝试升级内核。
3.12 查询无线网卡型号
1 个别无线网卡可能需要单独下载安装驱动：sudo lshw -c network
3.13 无线网卡加速
1 sudo deepin-editor /etc/modprobe.d/iwlwifi.conf
2 将11n_disable=1修改为11n_disable=0
3 重启电脑。
3.14 无线网卡解锁或蓝牙加锁
1 安装系统时或安装系统后无法驱动网卡，需要先排查笔记本是否有无线锁：检查键盘功能键。
2 查看：rfkill list
3 解锁无线：sudo rfkill unblock wifi
4 锁定蓝牙：sudo rfkill block bluetooth
3.15 判断缺少哪些硬件驱动
1 sudo update-initramfs -u
2 如发现有固件驱动缺失，可以从这个链接下载：
3 https://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware
.git/tree
4 之后放到/lib/firmware/对应目录下，并再次运行sudo update-initramfs -u更新。
5 注意：自己下载的固件在未来可能会跟系统新的固件包冲突，若是存在同名文件的话新固件包的
安装会报错，这时需要把之前下载的固件手动删除。
3.16 查询声卡信息
1 aplay -l
2 dmesg |grep snd
3 lspci |grep Audio
4 sudo lshw -c sound
Deepin UOS 深度技术群：19346666 24
第四章 Deepin 系统备份与还原
4.1 系统快照，折腾无忧
1 首先从应用商店搜索安装Timeshift，通过为系统制作快照，让系统还原到你想要的时间点。折
腾必备，强烈推荐！
2 快照类型：RSYNC，除非你的文件系统是btrfs。
3 位置：建议选择/home挂载的分区。
4 快照等级：建议禁用计划，或者勾选每月2次。推荐养成手动创建快照的好习惯，特别是当涉及更
新显卡驱动、内核等重要操作的时候。
5 用户：新手建议保持默认的“排除一切”。熟练后考虑选择“包含隐藏文件”并结合“筛选”可
更稳妥的折腾。
6 筛选：可随意添加，-号代表排除，+号代表添加。同一目录“排除在前，添加在后！”
7 例如我的筛选部分列表如下：
8 - /home/<用户名>/.deepinwine
9 - /home/<用户名>/.wine
10 - /home/<用户名>/.config/google-chrome
11 - /home/<用户名>/.cache
12 + /home/<用户名>/.**
13 - /root/**
14 配置完成后即可创建快照。
15 第一次快照需要完全备份，时间比较长，请耐心等待。之后凡是没修改的文件都只建立软链接，
速度就非常快了。
16 如果进不去桌面，可以在命令行下恢复。
17 查看：sudo timeshift --list
18 还原：sudo timeshift --restore
19 更多用法：timeshift --help
4.2 硬盘或分区克隆及恢复
1 推荐使用Clonezilla（再生龙）：http://www.clonezilla.org/
2 dd命令底层低效，仅供备用：
3 备份：sudo dd if=/dev/sda1 of=~/elf.bak status=progress
4 还原：sudo dd if=~/elf.bak of=/dev/sda1 status=progress
5 压缩备份：sudo dd if=/dev/sda1 status=progress | gzip -c > ~/elf.bak
6 压缩还原：gunzip -c ~/elf.bak | sudo dd of=/dev/sda1 status=progress
4.3 备份还原硬盘分区表
1 备份分区表：sudo sfdisk -d /dev/sdX > /path/to/fqb
2 还原分区表：sudo sfdisk /dev/sdX < /path/to/fqb
25
4.4 再生龙启动盘制作 第四章 DEEPIN 系统备份与还原
4.4 再生龙启动盘制作
1 Clonezilla（再生龙）官网：http://www.clonezilla.org/
2 官网速度较慢，建议从SF下载：https://sourceforge.net/projects/clonezilla/
files/
3 请下载适合USB存储介质的zip压缩包，例如clonezilla_live_stable目录下的clonezilla
-live-2.6.3-7-i686.zip
4 为U盘创建GPT格式分区表并创建两个分区，第二个分区300MB，用于存放Clonezilla再生龙启
动镜像，第一个分区占用U盘除EFI分区300MB外的所有空间，并格式化成exfat分区，用于
存放再生龙磁盘备份文件，也方便以后通过再生龙还原。U盘分区与格式化详见“跨平台可读
写文件系统exfat的格式化”小节。
5 将clonezilla-live-2.6.3-7-i686.zip解压到U盘第二个分区（FAT32）根目录下。
6 重启电脑，享用。
7 注意1：以上方法不适用传统MBR磁盘分区，MBR磁盘引导请参考：http://www.clonezilla.
org/liveusb.php
8 注意2: 之所以把EFI创建在第二个分区，是为了兼容Windows系统，该系统下U盘只支持一个分
区。
9 注意3: 如果想在macOS平台下格式化第一个分区，需要利用GParted把第二个分区标志设置为
“boot,esp”。此外，设置这个标志后，想使用第二个分区时，需要先手动挂载，Deepin
系统下推荐用“磁盘”应用挂载。
10 注意4: 再生龙默认会排除正在使用的磁盘，提示找不到U盘时，Ctrl+C跳过即可。
4.5 再生龙分区备份恢复到新硬盘
1 如果源磁盘数据HOME分区以及_dde_data数据盘占用空间过大或涉及个人隐私不便于单位共享
时，全盘备份就不适合了。
2 此时可以只备份EFI和ROOT分区，还原到新硬盘后适当的调整就可以正常使用。
3 1. 还原时选择“专家模式”，在“额外的高级参数”页面选择“-k1 照比例放大产生硬盘分割
表”；
4 2. 完成分区恢复后，进入命令列，执行：
5 sudo su && cd /home/partimag && ls
6 可以找到你U盘中分区备份所在目录，进入该目录并查看blkid.list文件，根据相应分区的
uuid重新格式化，例如：
7 mkswap -U a5fd6924-b890-44e9-b96c-ccbbf92be628 /dev/sda2
8 mkfs.ext4 -L Home -U beeb0e87-46f4-4a53-b828-6a2fda66a1b9 /dev/sda4
9 mkfs.ext4 -L _dde_data -U 5c86adb1-7cb3-4a39-81fb-490e748dd27d /dev/
sda5
10 重启后会发现无法登陆DDE，解决方法请参照“主目录被误删除的恢复方法”。
4.6 再生龙备份恢复到大容量磁盘
1 如果目标磁盘空间比源磁盘空间大，再生龙在恢复磁盘备份后，会导致目标磁盘有部分空间处于
未使用状态，浪费了。
2 解决方法：还原时选择“专家模式”，在“额外的高级参数”页面选择“-k1 照比例放大产生硬
盘分割表”。
Deepin UOS 深度技术群：19346666 26
第四章 DEEPIN 系统备份与还原 4.7 备份常见的用户配置
4.7 备份常见的用户配置
1 有时需要对$HOME主目录下的部分软件配置压缩备份，以便在另一台Deepin系统上解压还原，或
者格式化磁盘后恢复配置。
2 主目录下的配置文件默认是隐藏的，即以"."开头。显示这些隐藏文件的快捷键是Ctrl+H。
3 例如我会不定期压缩备份这些目录或文件：
4 $HOME/.config/autostart
5 $HOME/.config/Code/User/keybindings.json
6 $HOME/.config/Code/User/settings.json
7 $HOME/.config/google-chrome
8 $HOME/.config/shadowsocks-qt5
9 $HOME/.local/share/applications
10 $HOME/.local/share/fonts
11 $HOME/.ssh
12 $HOME/.vscode
13 $HOME/.gitconfig
14 $HOME/.profile
15 俗话说“有备无患”，重要资料、配置及时备份，可以提高学习、工作效率。
16 压缩包格式建议选择“.tar.xz”。
4.8 备份还原硬盘 MBR
1 备份MBR：sudo dd if=/dev/sdX of=/path/to/mbr bs=512 count=1
2 还原MBR：sudo dd if=/path/to/mbr of=/dev/sdX bs=512 count=1
3 MBR只还原分区表：sudo dd if=/path/to/mbr of=/dev/sdX bs=66 skip=446 count
=1
4 MBR清空引导记录：sudo dd if=/dev/zero of=/dev/sdX bs=446 count=1
Deepin UOS 深度技术群：19346666 27
4.8 备份还原硬盘 MBR 第四章 DEEPIN 系统备份与还原
Deepin UOS 深度技术群：19346666 28
第五章 Deepin 系统维护与技巧
5.1 开机进入命令行
1 开机进入命令行：sudo systemctl set-default multi-user
2 恢复开机进桌面：sudo systemctl set-default graphical
5.2 主目录被误删除的恢复方法
1 例如用户名是user，主目录/home/user，如果不小心把/home/user删除了，就会导致无法进
入DDE桌面，但可以进shell。
2 Ctrl+Alt+F2，进入tty2并登陆后，重新创建主目录并设置为当前用户所有：
3 sudo mkdir /home/user
4 sudo chown user /home/user
5 reboot重启。
5.3 解决与 Windows 时间不同步
1 sudo dpkg-reconfigure tzdata #时区设置
2 sudo hwclock --localtime --systohc #使用本地时间并写入主板
3 恢复UTC时间：sudo hwclock --utc --systohc
4 正常情况下，Deepin已经具备了网络时间同步功能，如一旦失效，则可以：
5 sudo apt install ntpdate #安装同步时间软件
6 sudo ntpdate-debian #网络时间同步
7 方法二：
8 timedatectl set-local-rtc 1 --adjust-system-clock
9 使用systemd启动之后，时间由timedatectl来管理，重启完成将硬件时间UTC改为CST。
10 timedatectl set-local-rtc 0 // 恢复UTC
11 查看：
12 cat /etc/adjtime
5.4 删除不需要的旧内核
1 查询所有内核：dpkg --get-selections |grep linux
2 正在使用的内核不能删除：uname -r
3 删除不需要的内核：sudo apt purge XXX
5.5 清除已卸载软件遗留配置
1 dpkg --get-selections |grep deinstall | sed 's/deinstall/\lpurge/' |
sudo dpkg --set-selections; sudo dpkg -Pa
29
5.6 假死后安全重启系统 第五章 DEEPIN 系统维护与技巧
5.6 假死后安全重启系统
1 Alt+SysRq+R-E-I-S-U-B，按住Alt+SysRq后再按顺序按一次后面六个字母。
2 可实现安全重启，其中SysRq就是Print Screen键。
3 REISUB可以按BUSY的比较级BUSIER倒写来记。
4 注意有Fn功能键的，视配置可能需要同时按住Fn功能键。
5 感谢bbs.deepin.org社区 @funtoo 指导：
6 R-从X11那里夺回键盘控制权
7 E-向所有进程发送SIGTERM信号
8 I-向所有进程发送SIGKILL信号
9 S-把待写入硬盘的数据同步到硬盘
10 U-将所有分区挂载为只读模式
11 B-重新启动
12 如果只是简单粗暴Alt+SysRq+B，有可能导致数据丢失等问题。
5.7 进程相关命令
1 pgrep XXX #查询进程ID
2 ps -ef |grep XXX #显示所有进程信息，连同命令行
3 ps -aux |grep XXX #列出目前所有的正在内存当中的程序
4 可以用 | 管道和 more 连接起来分页查看：ps -aux |more
5 sudo netstat -tulpn |grep :21 #查询端口
6 pkill XXX #杀掉
7 killall XXX #全杀
5.8 查看与同步 GPT 分区 UUID
1 查看UUID方法一：blkid
2 查看UUID方法二：ls -l /dev/disk/by-uuid
3 查看UUID方法三：lsblk -f
4 同步：sudo nano /etc/fstab
5.9 修改分区 UUID
1 sudo tune2fs -U c1b9d5a2-f162-11cf-9ece-0020afc76f16 /dev/sda5
2 sudo tune2fs -U random /dev/sda5
3 swap分区只能在LIVE环境通过mkswap -U修改。
5.10 sfdisk 创建磁盘 GPT 分区
1 命令：sfdisk /dev/sdX
2 其中X为你要操作的硬盘编号，例如a，对应/dev/sda
3 输入命令help可看到分区示例：“,200m”，表示创建第一个分区，大小200MB。
4 继续输入创建分区命令“,8g”并回车确认，可创建大小为8GB的第二个分区。
5 利用磁盘剩余空间创建最后一个分区时，只需输入逗号“,”并回车即可。
Deepin UOS 深度技术群：19346666 30
第五章 DEEPIN 系统维护与技巧 5.11 修改磁盘卷标
5.11 修改磁盘卷标
1 打开分区编辑器(GParted)软件，可以在磁盘格式化时设置所有支持格式的卷标。
2 如果不需要格式化，则可以先从“计算机”页面卸载目标分区，然后分区右键“重命名”，或者
通过“分区 - Label File System”完成卷标设定。
3 对于不支持GParted格式化的分区，例如exfat，可以通过命令行来设定：
4 sudo exfatlabel /dev/sdc1 USB
5 各种磁盘格式的卷标对应的修改命令如下：
6 # mlabel or fatlabel for fat32
7 # ntfslabel for ntfs
8 # exfatlabel for exFAT
9 # e2label for ext2/ext3/ext4
10 # btrfs for BTRFS
5.12 跨平台可读写文件系统 exfat 的格式化
1 首先，通过“分区编辑器(GParted)”右键卸载相应分区后为U盘创建GPT分区表，然后创建两个
fat32主分区并应用。
2 其次，需要用sudo fdisk -l查看磁盘或者分区信息，例如：
3 Disk /dev/sdb: 28.7 GiB, 30752000000 bytes, 60062500 sectors
4 ...
5 Device Start End Sectors Size Type
6 /dev/sdb1 2048 59447295 59445248 28.4G Microsoft basic data
7 /dev/sdb2 59447296 60061695 614400 300M Microsoft basic data
8 建议把第一个分区sdb1格式化成exfat格式，以便在Windows、macOS和Linux都可以支持大文
件读写。
9 建议把第二个分区sdb2分区作为EFI引导分区，大小300MB即可，将来做启动盘使用。
10 最后，将第一分区sdb1格式化成exfat磁盘格式：
11 sudo mkfs.exfat /dev/sdb1 -n USB
12 注意1：sdb1中的b和1因磁盘和分区数量不同而异，不要照搬，实际运用时需要酌情变更。
13 注意2：如果将整个U盘格式化为exfat格式，则可以：
14 sudo mkfs.exfat /dev/sdb
5.13 修改系统运行级别
1 当前级别查看：runlevel
2 0 系统停机模式，系统默认运行级别不能设置为0，否则不能正常启动，机器关闭。
3 1 单用户模式，root权限，用于系统维护，禁止远程登陆，类似Windows下的安全模式登。
4 2 多用户模式，没有NFS网络支持。
5 3 完整的多用户文本模式，有NFS，登陆后进入控制台命令行模式。
6 4 系统未使用，保留一般不用。
7 5 图形化模式，登陆后进入图形界面。
8 6 重启模式，默认运行级别不能设为6，否则不能正常启动。运行init 6机器就会重启。
9 更改运行级别：
10 sudo init 3
Deepin UOS 深度技术群：19346666 31
5.14 离线安装软件 第五章 DEEPIN 系统维护与技巧
5.14 离线安装软件
1 当没有网络连接的电脑上需要安装某个软件时，可以使用下面的脚本下载该软件以及依赖包，在
脱机电脑上执行：sudo dpkg -i *.deb
2 如果上述安装命令最后报错，则需要执行：sudo apt install -f
3 如果提示缺少软件包（依赖），则拷贝依赖包名（例如XXX），在有网络的电脑上执行
4 apt download XXX下载，再拷贝到脱机电脑上双击安装即可。
5 批量下载脚本如下：
6 #! /bin/bash
7 pkg="$*"
8 function getDepends()
9 {
10 ret=`apt-cache depends $1 |grep -i 依赖 |sed 's/(.*)//' |cut -d: -f2`
11 if [[ -z $ret ]]; then
12 echo "$1 No depends"
13 echo -n
14 else
15 # echo $ret
16 # apt-cache depends $1 |grep -i 依赖
17 # echo ''
18 for i in $ret
19 do
20 if [[ `echo $pkg |grep -e "$i "` ]]; then
21 # echo "$i already in set"
22 echo -n
23 elif [[ $i =~ '<' ]]; then
24 echo "Drop $i"
25 elif [[ "$i" != "libc6" &&
26 "$i" != "libcairo2" &&
27 !("$i" =~ "glib") &&
28 !("$i" =~ "gtk") &&
29 !("$i" =~ "font")
30 ]]; then
31 # echo "Download $i ing"
32 pkg="$pkg $i"
33 getDepends $i
34 fi
35 done
36 fi
37 }
38
39 for j in $@
40 do
41 getDepends $j
42 done
43
44 apt download $pkg -d -y
Deepin UOS 深度技术群：19346666 32
第五章 DEEPIN 系统维护与技巧 5.15 升级操作系统内核
5.15 升级操作系统内核
1 在Linux使用过程中，由于系统自带内核版本太老，或者存在一定程度的硬件支持缺陷，用户往
往会遇到诸如无线网卡信号不佳、网络连接不稳定、硬件设备无法识别和使用等问题。
2 如果您遇到了这些问题，可能就需要安装使用新版本内核来进行排查。
3 尽管新内核有可能解决部分硬件兼容问题，但是也有很大几率导致现有的闭源驱动无法正常使
用。
4 请只有在当涉及硬件驱动问题而走投无路的时候，才更换内核。
5 Linux内核和上层应用的耦合程度较低，所以一般不同发行版的内核可以通用。经测试，Ubuntu
的内核可以直接拿来给Deepin使用：
6 https://kernel.ubuntu.com/~kernel-ppa/mainline/
7 寻找你想使用的内核版本，例如5.4.28：
8 https://kernel.ubuntu.com/~kernel-ppa/mainline/v5.4.28/
9 一般只下载带"all"和"generic"字样的包，例如：
10 linux-headers-5.4.28-050428_5.4.28-050428.202003250833_all.deb
11 linux-headers-5.4.28-050428-generic_5.4.28-050428.202003250833_amd64.
deb
12 linux-image-unsigned-5.4.28-050428-generic_5.4.28-050428.202003250833
_amd64.deb
13 linux-modules-5.4.28-050428-generic_5.4.28-050428.202003250833_amd64.
deb
14 单独放在一个目录中，终端下执行：
15 sudo dpkg -i *.deb
16 重启，然后选择新内核引导项即可。
5.16 自行编译内核
1 一般只在需要自行调整内核编译参数时，才需要自己编译内核。这是个费时又费力的活。
2 1. 安装必备工具和依赖：sudo apt install build-essential fakeroot bison
flex libssl-dev libncurses5-dev
3 2. 下载内核源码：https://www.kernel.org/ ，选择版本，下载后右键“解压到当前文件
夹”。
4 3. 进入源码所在目录，右键“在终端中打开”，拷贝旧配置文件：cp /boot/config-`
uname -r`* .config
5 4. 基于当前系统内核配置文件生成新内核配置文件：make olddefconfig
6 5. 调整内核编译参数，除非你清楚选项的作用，否则请忽略：make menuconfig
7 6. 多核编译：make deb-pkg -j $(echo $(nproc)-1|bc)
8 7. 编译完成后，会在源码的上一级目录中生成deb安装文件，sudo dpkg -i *.deb 安装即
可。
9 注意：
10 1. 如果想修改参数再重新编译，建议执行”make mrproper“清理一下
11 2. 上述第四步不建议使用默认配置：make defconfig
12 3. 推荐阅读：https://www.jianshu.com/p/9fbdfd919fc0
5.17 重置所有用户配置
Deepin UOS 深度技术群：19346666 33
5.18 终端 CTRL+R 执行历史命令 第五章 DEEPIN 系统维护与技巧
1 该方法仅当出现疑难杂症无法解决时，才考虑采取的不得已的手段，可以将所有用户配置重置，
但也会丢失主目录下所有的资料。请在使用该方法前，一定要备份好主目录。这时就体现了
存在一个自动挂载的数据盘的重要性了。
2 方法是在终端执行命令：sudo init 3
3 系统重启后，会进入shell，登陆。比如用户名是user，则主目录是/home/user。
4 那么先手动删除主目录：sudo rm -rf /home/user
5 再重建主目录并获取所有权：
6 sudo mkdir /home/user
7 sudo chown user /home/user
8 重启reboot就行了。
9 注意：请务必替换上面命令的user为你当前系统正在使用的用户名。
10 注意：请一定要先备份好主目录的资料，否则找不回！
5.18 终端 Ctrl+R 执行历史命令
1 当在终端执行一些常用命令时，比较高效的做法是调用历史命令。执行快捷键Ctrl+R，输入需要
执行命令的一部分，找到需要的命令后，回车执行。
2 查看更多的历史命令：history 「所有历史命令都保存在~/.bash_history中」
5.19 更换用户名及家目录
1 终端执行sudo init 3进入shell，并以root账户登陆，之后执行：
2 usermod -l new_username -d /home/new_username -m old_username
3 groupmod -n new_username old_username
5.20 配置命令行默认 Python 版本
1 不推荐，可能导致某些依赖python的软件出现问题！在此仅作为示例，介绍update?alternatives的基本用法。
2 首先需要在系统中添加Python2.7、Python3.5的选项，默认为Python3.5（优先级20）
3 sudo update-alternatives --install /usr/bin/python python /usr/bin/
python2.7 10
4 sudo update-alternatives --install /usr/bin/python python /usr/bin/
python3.5 20
5 显示：update-alternatives --display python
6 切换：sudo update-alternatives --config python
5.21 软件包管理技巧
5.21.1 禁止某软件包升级
1 echo "XXX hold" | sudo dpkg --set-selections
2 apt-mark hold XXX
Deepin UOS 深度技术群：19346666 34
第五章 DEEPIN 系统维护与技巧 5.22 从源码编译安装软件包
5.21.2 允许某软件包升级
1 echo "XXX install" | sudo dpkg --set-selections
2 sudo apt-mark unhold XXX
5.21.3 修正 dpkg -i *.deb 安装后缺少依赖
1 sudo apt install -f
5.21.4 强制清除
1 sudo dpkg --purge --force-all XXX
5.22 从源码编译安装软件包
5.22.1 通过源码编译升级软件包
1 1. 安装公钥：sudo apt install debian-keyring #开发者公钥
2 2. 安装依赖：sudo apt build-dep XXX
3 3. 下载源码：apt source XXX
4 4. 替换源码或修改源码
5 5. 重新编译：cd 源码目录 && dpkg-buildpackage -rfakeroot -uc -b
6 6. 覆盖安装：sudo dpkg -i *.deb
7 第5步执行之前，可能需要先安装制作工具：sudo apt install fakeroot dh-make
5.22.2 基于源码编译 Shadowsocks-Qt5
1 1. 安装依赖
2 sudo apt install --no-install-recommends debhelper pkg-config qt5-qmake
qtbase5-dev libbotan1.10-dev libqrencode-dev libzbar-dev
libappindicator-dev
3 sudo apt install debhelper pkg-config qt5-qmake qtbase5-dev
4 2. 编译安装：https://github.com/shadowsocks/libQtShadowsocks
5 export PATH="/usr/lib/x86_64-linux-gnu/qt5/bin:$PATH"
6 dpkg-buildpackage -uc -us -b
7 sudo dpkg -i ../libqtshadowsocks*.deb ../shadowsocks-libqtshadowsocks*.
deb
8 3.编译安装：https://github.com/shadowsocks/shadowsocks-qt5
9 export PATH="/usr/lib/x86_64-linux-gnu/qt5/bin:$PATH"
10 dpkg-buildpackage -uc -us -b
11 sudo dpkg -i ../shadowsocks-qt5*.deb
Deepin UOS 深度技术群：19346666 35
5.23 文件或目录权限管理 第五章 DEEPIN 系统维护与技巧
5.23 文件或目录权限管理
1 点击文件或者目录右键菜单项”属性“，可在”权限管理“中分配特定权限。也可命令设定：
2 chmod 755 XXX
3 mode的三个数字，分别表示owner,group,others所具备的权限。
4 1＝x 执行，2＝w 写，4＝r 读
5 比如owner具有所有权限：1+2+4=7，而 group 具有读和执行权限：1+4=5。
6 命令ls -l可查看权限。
5.24 VirtualBox 虚拟机减肥
1 1.关闭虚拟机休眠功能：powercfg /h off
2 2.关闭系统还原
3 3.磁盘碎片整理
4 4.下载sdelete，执行：sdelete -c -z C: D:
5 5.关闭虚拟机
6 6.VBoxManage modifyhd --compact WIN7.vdi
5.25 安装 TeXLive 最新版
1 官网下载网络安装程序：http://tug.org/texlive/acquire-netinstall.html
2 精简安装: sudo apt install perl-tk && ./install-tl gui
3 安装选项：方案选择“small scheme”，便携安装并指定路径，选项默认A4纸，“创建所有格
式文件”选“是”，其余全部选“否”。
4 扩展宏包: tlmgr install exam xpatch titlesec zhnumber everypage
subfigure tcolorbox environ trimspaces wrapfig draftwatermark
synctex latexindent silence letltxmacro
5 中文宏集: tlmgr install ctex
6 免费字体：tlmgr install fandol
7 移除: tlmgr remove XXX
8 更新: tlmgr update --all
9 搜索: tlmgr search --global --file XXX
5.26 支持多架构：64 位系统安装 32 位软件
1 sudo dpkg --add-architecture i386
2 sudo apt update
3 sudo apt install XXX:i386
5.27 Backports 新版本软件安装
Deepin UOS 深度技术群：19346666 36
第五章 DEEPIN 系统维护与技巧 5.28 GIT 导出 WINDOWS 行尾源码
1 Deepin基于Debian 9,部分软件比较老旧，但可以通过添加Debian Backports源，来安装部
分软件的新版本。
2 参考网址：http://backports.debian.org/Instructions/
3 终端执行：sudo nano /etc/apt/sources.list.d/backports.list
4 添加内容：deb http://deb.debian.org/debian stretch-backports main
5 安装方法：sudo apt -t stretch-backports install "package"
6 更新列表：http://backports.debian.org/changes/stretch-backports.html
5.28 Git 导出 Windows 行尾源码
1 修改.git/config，添加：
2 [core]
3 autocrlf = true
4 eol = crlf
5 导出：
6 git archive -o export.zip HEAD
5.29 架设 TFTP 服务器
1 交换机、防火墙、路由器经常有网络备份配置、恢复配置的需求，这需要借助TFTP完成。
2 安装TFTP简易服务器：sudo apt install tftpd-hpa
3 配置：sudo nano /etc/default/tftpd-hpa
4 TFTP_USERNAME="<用户名>"
5 TFTP_DIRECTORY="/home/<用户名>"
6 TFTP_ADDRESS="0.0.0.0:69"
7 TFTP_OPTIONS="-l -c -s"
8 其中，loaden为当前登陆的用户名。
5.30 安装字体查看器
1 目前Deepin系统双击字体文件默认打开“字体安装器”，而无法查看字体详细信息。
2 建议安装字体查看器解决：sudo apt install gnome-font-viewer
5.31 nmap 端口扫描
1 建议：sudo apt install nmap
2 例如扫描指定UDP端口：sudo nmap -p 9902 -sU 10.35.99.100
3 反馈举例：9902/udp open|filtered unknown
4 扫描TCP端口举例：sudo nmap -p 9903 -sT 10.35.99.100
Deepin UOS 深度技术群：19346666 37
5.32 DNS 和 ARP 常用命令 第五章 DEEPIN 系统维护与技巧
5.32 dns 和 arp 常用命令
1 查询DNS：nslookup deepin.org
2 查询ARP：arp 或 cat /proc/net/arp
3 BSD风格显示：arp -a
4 清除arp缓存：sudo ip -s -s neigh flush all
5.33 chroot 切换后访问网络
1 以chroot /mnt为例，执行该命令后，可能会发现无法通过域名访问网络，原因是DNS解析服务
器不存在。
2 解决方法：在执行chroot命令前，拷贝Live的DNS解析。
3 即：sudo cp /etc/resolv.conf /mnt/etc/resolv.conf
5.34 tty 文本模式连接 wifi
1 作者：一本正经的胡说八道（QQ：1534646530）
2 Ctrl+Alt+F2进入tty2或sudo init 3进入文本模式，执行以下操作实现在终端连接wifi。
3 sudo NetworkManager start #确认NetworkManager服务开启
4 nmcli device wifi list #查看可连接的wifi列表
5 nmcli device wifi connect wifi-name password wifi-password #连接wifi
5.35 调整 GPT 磁盘分区顺序
1 GPT磁盘由于删减合并等，可能会导致分区设备数字错乱。
2 sudo cfdisk /dev/sdX，选择Sort，然后Write，输入yes完成重新排序命名，重启生效。
3 /dev/sdX视硬盘不同而修改，可sudo fdisk -l查看。
5.36 修改 SSH 端口号
1 nano /etc/ssh/ssh_config
2 默认端口为22,现修改成：Port 1979
3 重启服务：service sshd restart
4 连接：ssh -p 1979 root@qpsoft.com
5.37 利用 ssh 登陆服务器
1 ssh root@qpsoft.com
2 ssh -p 1979 root@qpsoft.com
Deepin UOS 深度技术群：19346666 38
第五章 DEEPIN 系统维护与技巧 5.38 利用 SSHFS 挂载主机文件系统
5.38 利用 sshfs 挂载主机文件系统
1 服务端：sudo apt install openssh-server #服务器默认已安装
2 客户端：sudo apt install sshfs
3 并加入fuse用户组：adduser <用户名> fuse
4 挂载：sshfs root@qpsoft.com:/ ~/.server
5 卸载：fusermount -u ~/.server
5.39 scp 在服务器和本地间传送文件
1 scp ~/somefile.tar.xz root@qpsoft.com:
2 scp root@qpsoft.com:test.tar.xz .
3 scp -r ~/somedirectory root@qpsoft.com:
4 scp -P 1979 some.tar.xz root@qpsoft.com:
5.40 开机出现 Firmware Bug 日志
1 错误日志内容：[Firmware Bug]: TSC_DEADLINE disabled due to Errata; please
update microcode to version: 0x22 (or later)
2 解决办法：sudo apt install intel-microcode 或 sudo apt install amd64-
microcode
3 检查安装：dmesg |grep microcode
4 问题来源：https://stackoverflow.com/questions/48036877/debian-firmware?bug-tsc-deadline-disabled-due-to-errata
5 应用这个补丁后，会降低CPU性能。家用不推荐。
5.41 ShadowSocks 代理上网
1 ShadowSocks软件自身配置完成后，还需要打开网络代理，配合VPS或者免费节点，才能科学上
网（推荐：electron-ssr）。
2 方法一：手动代理
3 控制中心-网络-系统代理-手动：SOCKS代理“127.0.0.1”,端口“1080”。
4 方法二：自动代理
5 控制中心-网络-系统代理-自动：配置URL“file:///home/<用户名>/.ss.pac”
6 sudo apt install python3-pip
7 sudo pip3 install genpac
8 genpac --pac-proxy "SOCKS5 127.0.0.1:1080" --gfwlist-proxy="SOCKS5
127.0.0.1:1080" --output=~/.ss.pac
5.42 不重启切换终端与桌面
1 不重启切换到终端：sudo systemctl isolate multi-user.target
2 从终端切换回桌面：sudo systemctl graphical.target
Deepin UOS 深度技术群：19346666 39
5.43 查询系统服务 第五章 DEEPIN 系统维护与技巧
5.43 查询系统服务
1 分类查询：systemctl list-units --type service --all
2 查询所有：systemctl list-unit-files
5.44 查询服务依赖
1 查询指定目标：systemctl list-dependencies multi-user.target
2 查询当前环境：systemctl list-dependencies
3 反向查询依赖：systemctl list-dependencies multi-user.target --reverse
5.45 创建服务延时执行命令
1 以下以创建一个执行1分钟后关闭错误报警蜂鸣声的服务为例，用到了at定时执行，需要提前安装
延时服务：sudo apt install at
2 说明：事实上，延时执行是没有必要的，仅以此为例，用户可尝试修改ExecStart的脚本。
3 sudo dedit /etc/systemd/system/nobeep.service
4 Requires=atd.service
5 添加内容：
6 [Unit]
7 Description=Keep quiet when some error happens
8 Requires=atd.service
9 [Service]
10 Type=simple
11 ExecStart=/bin/bash -c "echo /sbin/rmmod pcspkr |at now + 1 minutes"
12 [Install]
13 WantedBy=multi-user.target
14 启用自定义服务并测试判断：
15 sudo systemctl enable nobeep.service
16 systemctl list-dependencies nobeep.service --reverse
17 sudo systemctl start nobeep.service
18 systemctl status nobeep.service
Deepin UOS 深度技术群：19346666 40
第六章 Deepin 办公与生产力
6.1 必备的 WPS 兼容字体包
1 默认Linux版本WPS打开公文报表时，由于字体缺失，会导致不兼容Windows平台样式，体现不
出相同的展示效果。
2 字体介绍地址：http://wps-community.org/download.html?vl=fonts#download
3 字体下载地址：http://kdl.cc.ksosoft.com/wps-community/download/fonts/wps?office-fonts_1.0_all.deb
4 双击安装即可。如下载失败，请加QQ群19346666，从群文件“字体”目录下载。
6.2 PDF 文件压缩
1 gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/ebook -
dNOPAUSE -dQUIET -dBATCH -sOutputFile=output.pdf input.pdf
2 -dPDFSETTINGS=/screen 压缩比最大，输出文件最小，质量最低
3 -dPDFSETTINGS=/ebook 压缩比稍小，输出文件较小，质量稍高
4 -dPDFSETTINGS=/printer 高质量输出，文件较大
5 也可以-dColorImageResolution=180调整图像DPI：
6 gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dDownsampleColorImages=
true -dColorImageResolution=130 -dNOPAUSE -dBATCH -sOutputFile=
output.pdf input.pdf
6.3 卸载搜狗输入法，改用 Google 拼音
1 由于搜狗输入法存在严重的内存泄露（开机大约8小时，内存占用将达到3G)，在官方修复内存泄
露之前，建议替换成fcitx输入法。
2 卸载搜狗输入法：sudo apt purge fcitx* sogou*
3 完成卸载后，一定要注销或者重启。
4 杀掉所有fcitx进程：killall fcitx
5 确认这条命令没有任何输出了：pgrep fcitx
6 删除旧配置「注意！每行命令只有-r前后有空格，如果不理解，请图形界面手动删除」：
7 rm -r ~/.sogouinput
8 rm -r ~/.config/SogouPY*
9 rm -r ~/.config/sogou*
10 rm -r ~/.config/fcitx*
11 安装Google拼音输入法：
12 sudo apt install fcitx-googlepinyin
13 启动测试：
14 fcitx-autostart
15 如无报错，成功。
16 深入了解fcitx安装情况：fcitx-diagnose
41
6.4 安装中州韵 FCITX-RIME 输入法 第六章 DEEPIN 办公与生产力
6.4 安装中州韵 fcitx-rime 输入法
1 请卸载搜狗拼音输入法！为了避开奇怪问题，建议先彻底卸载fcitx和RIME输入法。
2 sudo apt purge fcitx* *rime*
3 sudo apt autoremove --purge
4 尝试重启或者注销电脑，也可尝试杀掉所有fcitx进程：killall fcitx
5 确认这条命令没有任何输出：pgrep fcitx
6 删除旧配置「注意！该命令只有-r前后有空格，如果不理解，请图形界面手动删除」：
7 rm -r ~/.config/fcitx
8 其中~代表主目录。
9 安装fcitx-rime：sudo apt install fcitx-rime
10 测试：fcitx-autostart
11 如果还无法使用中州韵，托盘输入法图标右键“配置”手动添加。
12 Ctrl+Alt+P可切换内嵌编辑模式（PreeditStringInClientWindow=False）。
13 下载配置、词库和皮肤：https://www.github.com/loaden/rime
14 覆盖到 ~/.config/fcitx/rime 目录下，托盘输入法图标右键菜单“重新部署”。
15 将 skin 目录移动到 ~/.config/fcitx 目录下可实现自定义皮肤。
16 输入法配置快捷键：Ctrl+` 或 Ctrl+Shift+` 或 Ctrl+0 或 F4。
17 常见用法详见：https://github.com/loaden/rime/blob/master/README.md
18 更多用法需要参考配置文件（含custom的yaml）中的注释。
6.5 安装中州韵 rime-ibus 输入法
1 请卸载搜狗拼音输入法！为了避开奇怪问题，建议先彻底卸载ibus和RIME输入法。
2 sudo apt purge ibus* *rime*
3 sudo apt autoremove --purge
4 尝试重启或者注销电脑，也可尝试杀掉所有ibus进程：killall ibus
5 确认这条命令没有任何输出：pgrep ibus
6 删除旧配置「注意！该命令只有-r前后有空格，如果不理解，请图形界面手动删除」：
7 rm -r ~/.config/ibus
8 rm ~/.xinputrc
9 其中~代表主目录。
10 然后安装ibus-rime: sudo apt install ibus-rime
11 测试：ibus-setup
12 由于deepin对im-config的错误修改，导致无法启用ibus，解决办法：
13 sudo rm -f /usr/share/im-config/data/21_ibus.*
14 终端运行：im-config，“确定”后选择“Yes”手动指定用户设置，弹出窗口中选择ibus后确
认，注销并重新登陆后，启动器搜索ibus或者托盘输入法图标打开“首选项”，在“输入
法”页面添加RIME。
15 下载配置、词库：https://www.github.com/loaden/rime ,覆盖到 ~/.config/ibus/
rime 目录下，托盘输入法图标左键单击菜单“部署”或右键“重新启动”。ibus-rime在
非GNOME桌面下，无法自定义皮肤，候选窗口左侧存在丑陋拖动条，底部出现多余上、下箭
头。如果你知道怎么解决这个问题，请不吝赐教。
16 建议在“iBus首选项 - 常规”里关掉“在应用程序窗口中启用内嵌编辑模式”，在“高级”里
关闭“在所有应用程序中共享同一个输入法”。如果找不到“iBus首选项”，可在终端执
行：ibus-setup
Deepin UOS 深度技术群：19346666 42
第六章 DEEPIN 办公与生产力 6.6 输入法无法开机自启动
6.6 输入法无法开机自启动
1 第1步：建议终端命令fcitx-diagnose检查有无异常报错。
2 第2步：建议终端命令im-config，“确定”后选择“Yes”手动指定用户设置，弹出窗口中选择
fcitx或者ibus后确认。
3 检查生成的配置文件：cat ~/.xinputrc 并确认配置文件生成时间和所自启动的输入法是否正
确。
4 注销并重新登陆。
5 第3步：如果仍然无法自启动，则可以针对fcitx输入法框架尝试终端命令：
6 echo -e "export GTK_IM_MODULE=fcitx\nexport XMODIFIERS=@im=fcitx\
nexport QT_IM_MODULE=fcitx" > ~/.xprofile
7 针对ibus输入法框架尝试终端命令：
8 echo -e "export GTK_IM_MODULE=ibus\nexport XMODIFIERS=@im=ibus\nexport
QT_IM_MODULE=ibus" > ~/.xprofile
9 然后重复第1步和第2步，注销后重新登陆。
10 如果仍然无法开机启动输入法，请重新安装im-config：sudo apt install im-config --
reinstall
11 然后重复第2步，注销后重新登陆。
6.7 解决中州韵偶尔无法输入中文
1 中州韵会偶尔出现无法输入中文的现象，之前只能重启输入法才能解决。
2 最新发现，只要Ctrl+` 或 Ctrl+Shift+` 切换一下输入法，比如我从“五笔86”切换到“五
笔拼音”即可解决。
6.8 搜狗输入法解决内存泄露
1 搜狗输入法2.3.1版本已经解决了内存泄露问题，喜欢搜狗输入法的朋友，只需要从官方下载安
装包更新：
2 https://pinyin.sogou.com/linux/?r=pinyin
3 因皮肤不兼容，建议卸载自带的五笔拼音：sudo apt purge fcitx-table-wbpy
4 安装完成后注销系统，重新登陆即可。
6.9 Blender 视频剪辑多核渲染插件
1 Blender 2.81a 版本视频剪辑功能已经非常强大，然而默认单核渲染，速度极慢是硬伤。通过
安装ktba插件可支持多核渲染，极大的提高了视频渲染速度。
2 插件地址：https://github.com/elmopl/ktba
3 使用帮助：https://github.com/elmopl/ktba/wiki/Addons
Deepin UOS 深度技术群：19346666 43
6.10 BLENDER 视频剪辑多核渲染崩溃处置 第六章 DEEPIN 办公与生产力
6.10 Blender 视频剪辑多核渲染崩溃处置
1 Blender视频剪辑多核渲染崩溃的解决方案：可以尝试取消Mixsound Sound选项，也可以使用
脚本手动连接与合并。
2 方法一：直接将包含音频的视频连接，详见群文件concat_contails_audio.sh，内容如下：
3 #!/bin/bash
4 for file in `find . -type f -a -name '*-*.mp4'`
5 do
6 buf=$buf"file '${file:2}'\n"
7 done
8 echo -e $buf |sed "/^$/d" |sort -t "-" -k 2n > in.txt
9 ffmpeg -f concat -i in.txt -c copy out.mp4
10
11 方法二：
12 先从Blender里渲染音频，例如in.mp3（如果是其它格式音频，需要修改脚本），它的原理是先
连接视频(丢弃音频），然后再把单独渲染的音频与之合并。
13 将方法一脚本的最后一条命令替换成：
14 ffmpeg -f concat -i in.txt -c:v copy -an in.mp4
15 ffmpeg -i in.mp4 -i in.mp3 -c:v copy -c:a copy out.mp4
16 rm in.mp4
17 详见群文件concat_merge_audio.sh。
6.11 ffmpeg 音频视频编码
6.11.1 ffmpeg 视频转换
1 ffmpeg -i input.mp4 -s:v 1280x720 -b:v 2000k -r:v 25 -c:v h264 -c:a ac3
-b:a 128k -r:a 44100 -ac 2 output.mp4
2 :v视频参数，:a音频参数，-ac声道。
6.11.2 批量编码转换
1 安装影音转换工具：sudo apt install ffmpeg
2 创建运行脚本：touch conv.sh
3 右键设置可执行权限，或者：chmod +x conv.sh
4 用编辑器打开conv.sh，添加以下内容（参数可酌情修改）:
5 #!/bin/bash
6 for file in `find . -type f -a -name '*.mov'`
7 do
8 ffmpeg -i "$file" -c:v h264 -b:v 3000k -r:v 25 -c:a ac3 -b:a 192k -r
:a 44100 -ac 2 "$(expr "$file" : '\(.*\)\.mov').mp4";
9 [ "x$?x" == "x0x" ] && rm "$file"
10 done
Deepin UOS 深度技术群：19346666 44
第六章 DEEPIN 办公与生产力 6.11 FFMPEG 音频视频编码
6.11.3 ffmpeg 视频连接
1 将需要连接的视频文件名根据自己需要的顺序放在in.txt文件中，每个文件一行：
2 file '0390-3917.mp4'
3 file '3918-7446.mp4'
4 连接视频和音频：ffmpeg -f concat -i in.txt -c copy out.mp4
5 只连接视频，丢弃音频：ffmpeg -f concat -i in.txt -c:v copy -an out.mp4
6 只连接音频，丢弃视频：ffmpeg -f concat -i in.txt -c:v none -c:a copy out.
mp3
6.11.4 ffmpeg 提取音频
1 知道视频中的音频编码时：ffmpeg -i in.mp4 -c:v none -c:a copy out.mp3
2 不知道编码，需要转换时：ffmpeg -i in.mp4 -c:v none -c:a ac3 -b:a 128k -r:a
44100 -ac 2 out.ac3
6.11.5 ffmpeg 视频混合音频
1 ffmpeg -i in.mp4 -i in.mp3 -c:v copy -c:a copy out.mp4
2 或简化成：ffmpeg -i in.mp4 -i in.mp3 -c copy out.mp4
3 in.mp4中的视频和音频与in.mp3中的音频混合输出。
6.11.6 ffmpeg 视频合并音频
1 ffmpeg -i in.mp4 -i in.mp3 -c copy -map 0:v -map 1:a out.mp4
2 in.mp4中的视频与in.mp3中的音频合并。
6.11.7 ffmpeg 截取视频
1 ffmpeg -i in.mp4 -to 5 -c copy out.mp4 #截取开头至第5秒
2 ffmpeg -i in.mp4 -ss 10 -c copy out.mp4 #截取第10秒至结束
3 ffmpeg -i in.mp4 -ss 6 -to 9 -c copy out.mp4 #截取第6秒至第9秒
4 ffmpeg -i in.mp4 -ss 8 -t 5 -c copy out.mp4 #从第8秒开始截取5秒
5 ffmpeg为了加速，会使用关键帧技术，所以有时剪切出来的结果在起止时间上未必准确。通常来
说，把-ss选项放在-i之前，会使用关键帧技术；把-ss选项放在-i之后，则不使用关键帧
技术。如果要使用关键帧技术又要保留时间戳，可以加上-copyts选项：
6 ffmpeg -ss 00:01:00 -i in.mp4 -to 00:02:00 -c copy -copyts cut.mp4
6.11.8 ffmpeg 指定时间合并
1 ffmpeg -ss 00:10:01 -t 30 -i in.mp4 -ss 00:05:02 -t 30 -i in.mp3 -c
copy -map 0:v -map 1:a out.mp4
2 in.mp4中第10分1秒开始的30秒视频与in.mp3中第5分2秒开始的30秒音频合并。
Deepin UOS 深度技术群：19346666 45
6.11 FFMPEG 音频视频编码 第六章 DEEPIN 办公与生产力
6.11.9 ffmpeg 调整播放速度
1 声音视频同时调节：ffmpeg -i in.mp4 -filter_complex -r 25 "[0:v]setpts
=1.25*PTS[v];[0:a]atempo=0.8[a]" -map "[v]" -map "[a]" out.mp4
2 只调节视频：ffmpeg -i in.mp4 -an -filter:v -r 25 "setpts=0.8*PTS" out.mp4
3 只调节音频：ffmpeg -i in.mp3 -filter:a "atempo=1.25" -vn out.mp3
Deepin UOS 深度技术群：19346666 46
第七章 Deepin 启动与多系统
7.1 开机画面卡死卡桌面或者黑屏
1 grub引导菜单界面，按e进入编辑模式（MBR磁盘按Tab键），修改“splash quiet”所在行，
在quiet之后添加：nouveau.modeset=0 或 nomodeset
2 或 nouveau.modeset=0 acpi_osi=! acpi="windows 2009"
3 或 nomodeset acpi_osi=! acpi="windows 2009"
4 注意添加上述参数时，前后留空格。按下F10应用新参数启动。
5 acpi="windows 2009"原理：据说是因为有些老旧的BIOS无法识别高版本的Linux内核，所以
grub加上这个参数就可以欺骗BIOS让它以为系统是windows7，然后就可以正常启动了。
6 如果还无法成功，可以尝试以下参数彻底禁掉nouveau开源驱动：
7 rd.driver.blacklist=nouveau modprobe.blacklist=nouveau nvidia-drm.
modeset=1
8 如果安装完成后相同参数引导卡LOGO，则可以尝试Ctrl+Alt+F2进入tty2终端安装显卡驱动。
9 如果无法进入tty2，请使用内核参数 systemd.unit=runlevel3.target 进 shell，之后
参考“硬件与驱动”章节在终端安装显卡驱动。
10 内核参数：https://wiki.archlinux.org/index.php/Kernel_parameters
7.2 启动后桌面空白，任务栏消失
1 安装完成后登陆系统，发现桌面只能看见壁纸，看不到任务栏。此时按下组合键Ctrl+Alt+T应
该可以显示终端。
2 判断当前分辨率是否正确：xrandr --curent
3 如果不正确，可以手动修改：xrandr -s 1920x1080
4 注意1920x1080之间的字母是英文xyz中的小写x，而不是乘号。
5 如仍然无法解决，尝试启动时加内核参数acpi=off
如果问题依然无法解决，请参考10.7章节。
7.3 系统启动分析
1 显示启动系统过程中用户态和内核态所花的时间：systemd-analyze
2 显示每个启动项所花费的时间明细：systemd-analyze blame
7.4 检查启动失败服务
1 安装新内核后可能出现systemd-modules-load.service加载失败，导致启动延时，原因是深
度开发的warm-sched延时加载功能的依赖驱动mincores在升级内核时编译失败。
2 可以用该命令检查启动失败的服务：
3 sudo systemctl --failed
47
7.5 查看开机日志 第七章 DEEPIN 启动与多系统
7.5 查看开机日志
1 首先使用systemd-analyze和systemd-analyze blame命令，对开机有个大致评估。
2 然后查看详细的启动日志：
3 sudo more /var/log/boot.log
4 最后查看启动过程中内核与硬件相关信息：
5 查看错误级别日志：sudo dmesg --level err
6 查看警告级别日志：sudo dmesg --level warn
7 更多级别或用法：dmesg --help
7.6 了解用户登陆情况
1 显示当前在本地系统上的所有用户的信息：
2 who 以及 whoami
3 列出目前与过去登入系统的用户相关信息:
4 last 以及 lastlog
7.7 利用系统安装盘进 Live 模式
1 插入烧录了Deepin系统的启动U盘，在启动菜单第一项“Install Deepin”高亮时按 e 进入
引导参数编辑状态。
2 将引导参数中的“livecd-installer”删除，F10启动即可进入Live桌面。
3 注意：由于没有闭源显卡驱动支持，进Live桌面后请仅限于系统维护、资料备份或GRUB引导修
复。要想体验优秀的DDE桌面环境，请实机安装。
7.8 Live 模式修复 GRUB 引导
1 进入Live模式后打开终端，或者安装盘进入安装界面时，Ctrl+Alt+F2进入tty2，先执行“
lsblk -f”找到系统安装分区sdaX，按顺序执行：
2 mount /dev/sdaX /mnt
3 mount /dev/sdaY /mnt/boot/efi
4 mount --bind /dev /mnt/dev
5 mount --bind /proc /mnt/proc
6 mount --bind /sys /mnt/sys
7 chroot /mnt
8 grub-install /dev/sda
9 update-grub
10 exit
11 sdaY为efi分区，MBR磁盘可忽略此步骤。重要：不同硬盘请酌情替换sda及X/Y。
12 注意：UEFI启动方式由于存在EFI分区，可以直接执行grub-install。
Deepin UOS 深度技术群：19346666 48
第七章 DEEPIN 启动与多系统 7.9 GRUB 维护技巧
7.9 GRUB 维护技巧
7.9.1 设置默认系统为用户选择
1 如果安装多系统，我们会有重启或开机时仍然进入上一次我们所选定系统的需求。
2 sudo nano /etc/default/grub
3 添加：
4 GRUB_DEFAULT=saved
5 GRUB_SAVEDEFAULT=true
6 更新：
7 sudo update-grub
7.9.2 隐藏启动菜单
1 sudo nano /etc/default/grub
2 添加：
3 GRUB_HIDDEN_TIMEOUT=1
4 GRUB_HIDDEN_TIMEOUT_QUIET=true
5 修改：
6 GRUB_TIMEOUT=0
7 更新：
8 sudo update-grub
9 长按Shift可以显示被隐藏的GRUB启动菜单，如果无效，可以开机长按ESC，进入grub命令行后
输入normal回车，然后再次按下ESC。
7.10 禁止 GRUB 检测其它系统
1 当配合第三方引导程序，例如Clover时，由于第三方引导界面已经展示了各系统的入口，所以
GRUB中没必要再保留其它系统入口了。
2 sudo apt purge os-prober
3 sudo rm -r /var/lib/os-prober/
4 sudo update-grub
7.11 屏蔽开关机屏幕日志
1 sudo nano /etc/default/grub
2 添加loglevel=2内核启动参数，例如：GRUB_CMDLINE_LINUX_DEFAULT="splash quiet
loglevel=2"
3 更新：sudo update-grub
4 该参数只是设置在屏幕上打印的内核日志级别，并不影响内核日志的记录。可用如下命令查看：
dmesg --level 3
5 详见：dmesg --help
Deepin UOS 深度技术群：19346666 49
7.12 开机关机巨大 LOGO 第七章 DEEPIN 启动与多系统
7.12 开机关机巨大 LOGO
1 安装Nvidia专有驱动后，很有可能会导致开机时，GRUB无法获取正确的分辨率。
2 sudo nano /etc/default/grub
3 添加：GRUB_GFXPAYLOAD_LINUX=keep
4 更新：sudo update-grub
5 如果GRUB2菜单分辨率仍然不正确，可尝试升级GRUB。
7.13 修正启动或关机界面分辨率
1 安装显卡专有驱动后，很有可能会出现开机时无法读取正确的分辨率，从而导致的巨大开机LOGO
。解决办法：
2 sudo nano /etc/default/grub
3 设置正确分辨率：
4 GRUB_GFXMODE=1920x1080
5 GRUB_GFXPAYLOAD_LINUX=keep
6 更新：
7 sudo update-grub
7.14 Ventoy 制作多系统启动盘
1 Ventoy可以实现在一个U盘上引导所有主流Linux系统、Windows系统进入安装程序，支持部分
PE。启动盘制作完成后，只需要将系统ISO镜像拷贝到U盘即可，支持Lagecy和UEFI两种方
式引导。该软件有Windows和Linux两个版本，简单易用。
2 Windows 7系统需要使用在原版镜像基础上集成微软官方USB3.0内核补丁和官方EFI引导程序的
修改版：https://pan.baidu.com/s/1D0ATxmhsbLtTH92-f9SgaQ 密码: oljr
3 强烈推荐这个国人开发的开源软件：http://www.ventoy.net
7.15 Win10 USB 启动盘制作
1 如果是Win10 LTSC，则只需将U盘用GPT分区表格式化成FAT32，然后在ISO镜像文件上右键
“打开方式”，选择“磁盘映像挂载器”。挂载成功后，将ISO磁盘内所有文件拷贝到U盘就
可以引导安装Win10了。
2 当然，在应用商店安装WoeUSB，也可以在图像界面下轻松制作Windows启动U盘。
3 如果是Win10 Business版本，由于FAT32格式文件大小4G限制，只能用WoeUSB在命令行下制
作Win10 USB启动盘：
4 sudo woeusb --target-filesystem NTFS --device
cn_windows_10_business_editions_version_1903.iso /dev/sdb
5 其中/dev/sdb通过sudo fdisk -l查询得到。
6 注意：无论是WoeUSB图形界面还是命令行操作，都需要先用“分区编辑器”把U盘卸载。
Deepin UOS 深度技术群：19346666 50
第七章 DEEPIN 启动与多系统 7.16 安装 DEEPIN 与 WINDOWS 双系统
7.16 安装 Deepin 与 Windows 双系统
1 情况一：如果是MBR传统格式的磁盘「Legacy」，先安装的Windows，后安装Deepin的话，默
认一定会出现GRUB引导菜单。
2 情况二：如果是MBR传统格式的磁盘「Legacy」，但是先安装的Deepin，后安装Windows，则
需要进LIVE重建GRUB引导。
3 情况三：如果是GPT新格式磁盘「UEFI」，先安装的Windows，后安装Deepin，则需要在BIOS
中将Windows Boot Manager用减号将优先级调到最低。
4 情况四：如果是GPT新格式磁盘「UEFI」，但是先安装的Deepin，后安装Windows，则需要安
装Windows后进Deepin更新GRUB。
5 注意一：如果UEFI安装Windows7与Deepin双系统，则只有启用CSM兼容模式才能启动Win7系
统。当启用CSM兼容模式时，将无法调整GPT各分区启动的优先级，如果后安装Deepin，会
导致重启直接进入Windows，不出现GRUB启动菜单，F12中的BIOS启动菜单也只有
Windows Boot Manager，无法进入Deepin系统。解决办法是先进BIOS关闭CSM，然后重
启还进入BIOS并设置Deepin所在分区为最高启动优先级，保存BIOS设置，再次重启进入
BIOS并打开CSM兼容模式。第三次重启，此时就能看到GRUB引导菜单了。
6 注意二：最省心的双系统安装BIOS设置是“UEFI Only”+“CSM Disabled”+“Secure
Boot Disabled”。
7.17 双系统修复 Windows EFI
1 Windows启动盘引导进入安装界面，点击“下一步”，再点击左下角“修复计算机”。
2 点击“疑难解答”，进入“命令提示符”，并根据上一节“Windows系统读写EFI分区”说明挂
载EFI分区。执行list volume查查看盘符，并记下系统盘符和EFI启动分区盘符。执行
exit退出diskpart。
3 例如我的Windows系统盘符为C，EFI启动分区盘符为F，则可以这样修复：
4 bcdboot C:\Windows /s F: /f uefi /l zh-cn
5 可以确认：dir F:\EFI，能看到Microsoft目录说明成功。
7.18 Windows 系统读写 EFI 分区
1 cmd中运行diskpart， 可通过以下命令为EFI分区分配盘符。
2 查看硬盘：list disk
3 选择硬盘：select disk 0
4 查看分区：list partition
5 选择分区：select partition 1
6 分配盘符：assign
7 右键以管理员身份运行notepad，“文件”-“打开”，就可以读写EFI分区了。
7.19 制作 USB 启动盘
1 sudo dd if=/path/to/the/downloaded/iso of=/path/to/the/USB/device
2 显示进度：
3 sudo dd if=/path/to/the/downloaded/iso of=/path/to/the/USB/device
status=progress
Deepin UOS 深度技术群：19346666 51
7.20 EFI 引导分区不要删除 UBUNTU 第七章 DEEPIN 启动与多系统
7.20 EFI 引导分区不要删除 ubuntu
1 EFI引导分区下同时存在deepin和ubuntu两个文件夹，无论你是否安装了Ubuntu系统。
2 原因是Ubuntu有硬件厂商的安全认证证书，而deepin暂时还没有，所以只能依赖Ubuntu的证书
来通过grub引导启动了。
3 删除ubuntu目录将无法启动Deepin！
4 修复方法：手动创建ubuntu目录并从同级deepin中拷贝grubx64.efi和grub.cfg。
7.21 误删 EFI 分区后的还原
1 第一步：利用Deepin安装盘进入LIVE并修复引导，此时ls /boot/efi/EFI可以看到已经生成
deepin目录，但还无法引导系统。
2 第二步：sudo cp -r /boot/efi/EFI/deepin /boot/efi/EFI/ubuntu
3 该指令的可靠性可以apt download grub-efi-amd64-signed后解压证实。
7.22 恢复 Deepin 引导主题
1 UEFI启动方式，如果先安装Deepin后安装Ubuntu形成双系统时，即使在Deepin系统下执行
grub-install，也会使用Ubuntu的GRUB引导菜单主题。
2 原因是Deepin依赖Ubuntu的安全引导。解决办法：
3 sudo cp /boot/efi/EFI/deepin/grub.cfg /boot/efi/EFI/ubuntu/grub.cfg
4 sudo grub-install
7.23 命令行查看 EFI 启动项
1 在终端执行命令：efibootmgr
2 显示：
3 BootCurrent: 0002
4 Timeout: 1 seconds
5 BootOrder: 0001,0000,0002,0013,0014,0015,0016,0012,0017
6 Boot0000* deepin
7 Boot0001* debian
8 Boot0002* uos
9 Boot0012* UEFI: SanDisk
10 Boot0013 ubuntu
11 Boot0014* UEFI OS
12 Boot0015 ubuntu
13 Boot0016* UEFI OS
14 Boot0017* UEFI: SanDisk
15 BootCurrent标号为2，指当前系统为uos，*代表有效启动，BootOrder代表启动顺序。
16 更多用法可查询：efibootmgr --help
Deepin UOS 深度技术群：19346666 52
第七章 DEEPIN 启动与多系统 7.24 查看当前 EFI 启动项详情
7.24 查看当前 EFI 启动项详情
1 efibootmgr -v
2 bootctl
7.25 删除重复的 EFI 启动项
1 sudo efibootmgr -D
7.26 调整 EFI 启动项顺序
1 sudo efibootmgr -o X,Y #指定标号为X的启动项顺序在Y之前
2 例如：sudo efibootmgr -o 0002,0001
7.27 创建 EFI 启动项
1 默认/dev/sda：sudo efibootmgr -c -L test -l "\EFI\uos\grubx64.efi"
2 指定/dev/sdb：sudo efibootmgr -c -L test -l "\EFI\debian\grubx64.efi" -d
/dev/sdb
7.28 删除 EFI 启动项
1 sudo efibootmgr -B -b 0003
7.29 查看硬盘分区信息
1 sudo parted -l
2 sudo fdisk -l
3 lsblk
4 blkid
5 df -h
7.30 修复黑苹果 Clover 引导
1 添加引导：sudo efibootmgr -c -L Clover -l "\EFI\CLOVER\CLOVERX64.efi"
2 查看并调整顺序：efibootmgr -v
3 详见“调整EFI启动项顺序”等。
Deepin UOS 深度技术群：19346666 53
7.31 LIVE 模式调整磁盘分区大小 第七章 DEEPIN 启动与多系统
7.31 Live 模式调整磁盘分区大小
1 进入Live模式后，运行启动器“GParted”，可以调整磁盘分区大小。
2 请耐心等待，调整完成后如果无法启动，则还需要修复磁盘文件系统，例如：
3 fsck.ext4 /dev/sda3
4 其中/dev/sda3为ROOT所在分区，请根据实际情况酌情修改。
7.32 Live 模式防锁屏后无法登陆
1 Debian的Live系统用户密码是live，但Deepin Live User密码却好像是随机的字符。
2 通过命令users可以查到用户名为deepin，但密码不是deepin，也不是live。
3 通过Deepin安装盘进入Live系统后，如果要长时间操作，例如调整磁盘分区，则可能会在15分
钟后自动锁屏，这时就没有办法进入DDE桌面了。
4 解决方法：Ctrl+Alt+F2，进入tty2，执行sudo su拿到管理员权限后，修改用户密码：
5 passwd deepin
6 密码修改完成后，Ctrl+Alt+F1切换到登陆界面，输入刚才修改的密码登陆。
7 要防止这种情况出现的办法：“控制中心”-“账户”选择“无密码登陆”；“电源管理”取消
“唤醒显示器时需要密码”和“待机恢复时需要密码”。
7.33 解决多系统启动缓慢
1 多Linux系统如果共用同一个swap交换空间，因为在安装新的Linux系统时，会自动格式化swap
交换空间，导致其uuid发生变化，与之前安装的Linux系统/etc/fstab自动挂载表中记录
的swap uuid不一致，所以导致启动长时间寻找swap分区。用systemd-analyze命令查
看，会发现userspace使用了大量时间。
2 解决方法：修改/etc/fstab，让swap分区与新的uuid同步。
7.34 VirtualBox 从 U 盘启动
1 第一步，用lsblk确定U盘设备名称，例如：/dev/sdc
2 第二步，为其它用户添加U盘读写权限：sudo chmod o+rw /dev/sdc
3 第三步，创建U盘虚拟磁盘文件：VBoxManage internalcommands createrawvmdk -
rawdisk /dev/sdc -filename ~/UDISK.vmdk
4 第四步，创建虚拟机后，设备-存储：“控制器”右键添加硬盘，并注册刚才创建的U盘虚拟磁盘
5 第五步，启动虚拟机，F12键：选择第2硬盘启动。
Deepin UOS 深度技术群：19346666 54
第八章 Deepin 远程控制与共享
8.1 向日葵远程控制
1 国产远程控制软件：https://sunlogin.oray.com
2 在网络封锁日益严重的今天，国产可能是唯一的选择。
8.2 TeamViewer 远程控制
1 安装：sudo apt install teamviewer
2 安装后即可于启动器中“TeamViewer”快捷方式启动，建议注册用户，登陆后将经常需要远程
控制的设备添加到用户。
3 TeamViewer请勿连接过多主机，否则很可能被判断为商用。
8.3 AnyDesk 远程控制
1 安装：sudo apt install anydesk
2 安装后即可于启动器中“AnyDesk”快捷方式启动，支持Windows、macOS、Linux、Android
、iOS等几乎全平台远程桌面连接。支持ID或者IP连接。
3 官方网站：https://anydesk.com/
4 目前AskDesk在自动启动后的权限上有些问题。
8.3.1 提高 AnyDesk 远程控制权限
1 设置›安全›交互连接：选择“始终允许”。经此设置后，访问Windows 7以上系统时，当开启
UAC的情况下，也能获得操作权限。
8.3.2 AnyDesk 自动连接控制
1 默认AnyDesk是需要被控端接受连接的，但通过“自主访问”选项，可以实现自动连接。
2 设置›安全›自主访问：选择“允许自主访问”，并输入连接密码。
8.3.3 禁止 AnyDesk 自启动
1 禁止自启动：sudo systemctl disable anydesk
2 恢复自启动：sudo systemctl enable anydesk
8.4 VNC 远程控制
1 应用商店搜索VNC，可以安装“VNC Viewer”和“VNC Server”两款软件，分别对应客户端和
服务端。
2 官方主页可下载最新安装包：https://www.realvnc.com
55
8.5 RDP 协议连接 WINDOWS 远程桌面 第八章 DEEPIN 远程控制与共享
8.5 RDP 协议连接 Windows 远程桌面
1 应用商店搜索 Remmina ，安装即可连接Windows远程桌面。
8.6 Linux 打印机共享
1 服务端：“启动器”-“打印设置”，从菜单“服务器”-“设置”中勾选“发布连接到这个系统
的共享打印机”和“允许从互联网打印”。默认被添加的本地打印机是处于共享状态的，可
以通过相应打印机右键菜单确认。
2 客户端：“启动器”-“打印设置”-“添加”，“查找网络打印机”页面输入打印机服务器地
址，即可找到IPP协议的网络打印机。
3 例如服务器地址为10.1.1.1，则搜索出来的打印机“输入设备URI”为：
4 ipp://10.1.1.1:631/printers/HP_LaserJet_M1005
5 前进，应用，打印测试页确认是否成功。
6 补充1：“打印设置”是CUPS打印机管理服务的图形化管理工具，可在/etc/cups/cupsd.
conf看到全部配置。
7 补充2：请不要选择SMB打印机共享，地址类似：smb://10.1.1.1/HP_LaserJet_M1005
8 补充3：“允许远程管理”与“允许从互联网打印”两个选项冲突，只能二选一。
8.7 Windows 打印机共享
1 服务端：与“Linux打印机共享”配置相同，区别只是客户端。
2 客户端：需要执行以下步骤
3 1. 安装打印机的Windows驱动，当弹出“请通过USB线连接打印机之类”的提醒时，说明驱动已
经安装成功，取消退出安装界面即可。
4 2. “设备和打印机”-“添加打印机”-“添加网络打印机”，点击“我需要的打印机不在列表
中”，从“按名称选择共享打印机”的输入框中填写打印机地址，类似：
5 http://10.1.1.1:631/printers/HP_LaserJet_M1005
6 下一步，在弹出的窗口中选择品牌和型号即可。
8.8 Windows 云打印共享
1 服务端：Windows上安装Deepin官方提供的“深度云打印”服务软件，可从QQ群19346666群文
件下载。USB连接打印机并安装驱动。
2 客户端：“启动器”-“深度云打印配置助手”，通过打印服务器地址和授权码连接。
3 备用下载地址：https://pan.baidu.com/s/1bofTyoR
Deepin UOS 深度技术群：19346666 56
第九章 Deepin 运行 Windows 软件
9.1 安装运行 Windows 绿色软件
1 进入绿色软件所在目录，右键“在终端中打开”，执行：
2 deepin-wine Windows绿色软件.exe
9.2 为大型 Windows 软件创建独立运行环境
1 建议每个大型软件使用一个独立的容器（运行环境），下面以安装Rosetta Stone为例。
2 第一步：拷贝或者创建容器
3 cp -r ~/.deepinwine/Deepin-QQ ~/.rosetta 或者
4 WINEPREFIX=~/.rosetta deepin-wine winecfg
5 第二步：安装
6 WINEPREFIX=~/.rosetta deepin-wine RosettaStone5.0.37.exe
7 如遇安装或者运行异常，可调试：
8 WINEDEBUG=+pid,+tid,+process WINEPREFIX=~/.rosetta deepin-wine $HOME'/.
rosetta/drive_c/Program Files/Rosetta Stone/Rosetta Stone Language
Training/Rosetta Stone.exe'
9 参考官方维基：https://wiki.deepin.org/wiki/Deepin-wine
10 注意：64位程序需要安装wine64，效果不佳。
9.3 修改 QQ 聊天窗口文字大小
1 如果觉得QQ聊天窗口字体太小了，可以打开终端，执行：
2 WINEPREFIX=~/.deepinwine/Deepin-QQ deepin-wine winecfg
3 弹出窗口中切换到“显示”页面，“屏幕分辨率”增大dpi，确定重启。
9.4 双击运行 Windows 软件
1 进入主目录，文件管理器Ctrl+H显示隐藏文件，进入.local/share/applications目录。
2 创建文件：deepinwine.desktop，添加如下内容并保存：
3 [Desktop Entry]
4 Categories=System;Utility;
5 Exec=/usr/bin/deepin-wine %F
6 Name=Wine
7 Terminal=false
8 NoDisplay=true
9 MimeType=application/x-ms-dos-executable;
10 Type=Application
11 然后在Windows的exe可执行文件上右键，“打开方式”选择Wine作为默认程序。
57
9.5 适配绿色版 PHOTOSHOP CC 第九章 DEEPIN 运行 WINDOWS 软件
9.5 适配绿色版 Photoshop CC
1 1.删除DeepinQQ旧容器：rm -rf ~/.deepinwine/Deepin-QQ
2 2.启动器运行QQ，等待出现登陆界面后再关闭
3 3.删除默认旧容器：rm -rf ~/.wine
4 4.借Deepin-QQ容器可避免标题乱码：cp -r ~/.deepinwine/Deepin-QQ ~/.wine
5 5.修改为Windows 7系统：deepin-wine winecfg
6 6.安装Phoneshop CC绿色版（thx Ansifa）
9.6 卸载 Windows 软件
1 首先下载绿色卸载软件：https://geekuninstaller.com/download
2 默认容器：双击geek.exe即可
3 指定容器：WINEPREFIX=~/.rosetta deepin-wine geek.exe
4 简单粗暴：rm -rf ~/.rosetta
Deepin UOS 深度技术群：19346666 58
第十章 Deepin 疑难问题解答
10.1 安装 Deepin 时找不到 M.2 硬盘
1 当主板使用M.2接口，NVMe协议的固态硬盘时，会导致安装Deepin时无法找到硬盘。尝试：
2 1. 将硬盘模式从RAID更改为AHCI。
3 2. 禁用”M.2/Optane Genie“选项。当M.2/Optane Genie设置为开启时，它将在安装时
支持Intel傲腾[Optane]内存，并在安装2个或者更多M.2设备时支持RAID功能。
10.2 应用程序假死或无响应
1 由于Deepin的窗口管理器偶尔会导致弹出窗口已经获得焦点，但却并没有显示在所有窗口的最前
端，此时会导致应用程序无法响应鼠标事件，让用户误以为程序假死或者无响应，导致不得
不关闭应用后重启。
2 解决方法：按ESC键，或者先按住ALT键，再按下TAB键，将失去响应的应用程序相关的弹出窗口
关闭。这些弹出窗口一般都是打开文件或者保存文件窗口。
10.3 禁用 IPv6 解决 QQ 图片显示
1 添加内核参数彻底禁用IPv6：sudo dedit /etc/default/grub
2 在此行添加参数：GRUB_CMDLINE_LINUX="ipv6.disable=1"
3 保存退出后执行：sudo update-grub
10.4 从 3D 游戏返回后屏幕闪烁
1 15.11版本发布时，官方宣称这两个问题已经解决。
2 * 修复多次切换3D/2D模式后打开新的有标题栏的窗口时会导致屏幕闪烁的问题；
3 * 修复多次切换3D/2D模式后打开新的有标题栏的窗口时其它未激活窗口的阴影显示为黑色；
4 实际未解决，升级内核至5.1.20，Nvidia驱动至430.34问题依然存在。
5 重启后问题可消失，改成deepin-wm窗口管理器问题也消失。
6 说明是KWin的锅。
7 临时解决办法：注销或者重启DDE桌面。
8 sudo service lightdm restart
9 或者：
10 sudo systemctl restart lightdm
59
10.5 关闭错误报警蜂鸣声 第十章 DEEPIN 疑难问题解答
10.5 关闭错误报警蜂鸣声
1 检查模块是否启动：lsmod |grep pcspkr
2 临时关闭：sudo rmmod pcspkr
3 永久关闭：
4 方法一：
5 deepin-editor ~/.profile 添加下面三行内容
6 sudo -S rmmod pcspkr <<EOF
7 password(你的密码)
8 EOF
9 在Shell脚本中，通常将EOF与 << 结合使用，表示后续的输入作为子命令或子Shell的输入，
直到遇到EOF为止，再返回到主Shell,即将‘你的密码’当做命令的输入。
10 方法二：
11 sudo deepin-editor /etc/modprobe.d/nobeep.conf 添加 blacklist pcspkr
12 经测试，虽然pcspkr不再自启动，但电脑启动时会发出奇怪噪音，错误报警声仍然存在。
13 备注：
14 如果开机画面屏幕输出”Driver 'pcspkr' is already registered“则可用方法二解
决。
10.6 睡眠/休眠唤醒之后触摸板失灵
1 作者：ChenHacker（QQ：2041026133）
2 链接：https://www.luogu.com.cn/blog/ChenHacker/linuxsleep
3 问题原因:
4 Linux的触摸板驱动是启动内核作为一个模块加载的，睡眠的时候可能由于Linux内核的bug这个
模块坏掉了，所以需要重新加载，而我们知道Linux系统中重新加载内核模块的方法是:
5 sudo modprobe -r *** #移除模块
6 sudo modprobe *** #加载模块
7 经过我几个小时的摸索，得知我的笔记本触摸板驱动的模块是i2c_hid(部分笔记本是psmouse)
，所以当唤醒睡眠之后执行一下命令我的触摸板就可以工作了。
8 sudo modprobe -r i2c_hid && sudo modprobe i2c_mid
9 但是每次睡眠之后都要打开终端执行这个命令，在Linux下怎么可以这么繁琐？？？
10 所以我们通过修改/usr/lib/systemd/system/systemd-suspend.service文件来解决。
11 这个文件是有关休眠服务的文件,也就是当你按下睡眠键时,系统就会执行这个文件。
12 我们先写好自己的睡眠文件：/usr/lib/systemd/system/mysleep
13 #!/bin/bash
14 /usr/lib/systemd/systemd-sleep suspend && modprobe -r i2c_hid &&
modprobe i2c_hid
15 添加可执行权限：sudo chmod +x /usr/lib/systemd/system/mysleep
16 然后修改/usr/lib/systemd/system/systemd-suspend.service文件中的对应选项：
17 [Service]
18 Type=oneshot
19 ExecStart=/usr/lib/systemd/system/mysleep
20 刷新系统服务:
21 sudo systemctl daemon-reload
22 然后这个问题就被根治了!
Deepin UOS 深度技术群：19346666 60
第十章 DEEPIN 疑难问题解答 10.7 任务栏/启动器消失
10.7 任务栏/启动器消失
1 终端执行命令：rm -rf $HOME/.config/dconf
2 或者文件管理器进入主目录，Ctrl+H显示隐藏文件后手动删除.config/dconf目录。
3 重新启动。
10.8 窗口无响应或系统卡顿
1 首先请确认已经安装了正确的显卡驱动：目前KWin仍然是官方默认的窗口管理器，但需要正确的
显卡驱动支持。如果依然出现窗口无响应或系统卡顿，可以尝试Super+Shift+Tab快捷键
两次：先关闭窗口特效，再打开窗口特效。
2 如果上述问题经常出现，可以牺牲部分特效，切换成2D窗口管理器，依次执行：
3 sudo apt install deepin-metacity
4 sudo apt purge dde-kwin
5 重启后用neofetch确认WM: Metacity。
10.9 创建 DEB 安装包
1 以打包软件包test为例，首先创建test/DEBIAN/control文件，必备内容：
2 Package: name
3 Version: 1.0-1
4 Architecture: amd64
5 Maintainer: 维护者 <user@mail.com>
6 Description: 简介
7 软件包详细介绍。
8 然后打包 dpkg-deb -b test 即可。
9 建议生成MD5：find ./usr -type f |xargs -I{} md5sum {} >DEBIAN/md5sums
10 配合脚本postinst、prerm可实现安装配置与卸载清理。
Deepin UOS 深度技术群：19346666 61
10.9 创建 DEB 安装包 第十章 DEEPIN 疑难问题解答
Deepin UOS 深度技术群：19346666 62
第十一章 Deepin 终端操作技巧集锦
11.1 以管理员身份自启动
1 编辑 ~/.profile 添加下面三行内容：
2 sudo -S rmmod pcspkr <<EOF
3 password(你的密码)
4 EOF
5 在Shell脚本中，通常将EOF与 << 结合使用，表示后续的输入作为子命令或子Shell的输入，
直到遇到EOF为止，再返回到主Shell，即将‘你的密码’当做命令的输入。
11.2 递归更改文件所有者
1 chown -R <用户名>:<用户名> *
11.3 从指定类型文件中查找
1 find . -name '*.c' | awk '{print "grep -i -nH keyword "$1}' | /bin/bash
2 find . -name '*.c' -exec grep -i -nH "keyword" {} \;
11.4 更好的搜索方法
1 grep -i "search_string" . -r --include=*.txt
2 grep "search_string" . -r --include=*.txt --include=*.cpp --include=*.h
11.5 将行末多个空行转换成一个空行
1 find . -name '*.tex' -exec sed -i '/^$/{N;/^\n*$/D}' {} \;
11.6 ls 只显示目录名
1 ls -l |grep ^d 或 ls -d */
11.7 ls 只显示文件
1 ls -l |grep ^-
63
11.8 LS 显示软链接 第十一章 DEEPIN 终端操作技巧集锦
11.8 ls 显示软链接
1 ls -n
11.9 为子目录和文件设置不同权限
1 find . -type d -exec chmod 755 {} \;
2 find . -type f -exec chmod 644 {} \;
11.10 为指定类型文件设置可执行权限
1 find . -name 'commit-msg' -type f -exec chmod +x {} \;
2 find . -name '*.sh' -type f -exec chmod +x {} \;
11.11 获取脚本文件所在路径
1 包含文件：$0
2 只要路径：`dirname "$0"`
11.12 批量文本替换
1 grep "old" -rl ./ |xargs sed -i "s/old/new/g"
2 grep "Objbase.h" -rl . --include=*.cpp --include=*.h |xargs sed -i "s/
Objbase.h/objbase.h/g"
3 或：
4 sed -i "s/原字符串/新字符串/g" `grep 原字符串 -rl 所在目录
5 举例：
6 grep "图像" -rl . --include=*.tex |xargs sed -i "s/图像/图象/g"
11.13 获取 CPU 个数并四则运算后导出环境变量
1 export MAKE_JOBS=$(echo $(nproc)-1|bc)
2 应用：make -j $MAKE_JOBS
11.14 命令行解压缩到指定目录
1 tar xvf XXX.tar.xz -C /opt
2 不需要添加J选项，tar会根据压缩包名称识别压缩包格式。
3 所以xvf应该可以作为万能参数了。
Deepin UOS 深度技术群：19346666 64
第十一章 DEEPIN 终端操作技巧集锦 11.15 通过 GIT 实现跨平台的 GREP 用法
11.15 通过 git 实现跨平台的 grep 用法
1 git grep -li pkgconfig -- \*.pr?
11.16 打印当前目录路径
1 pwd
11.17 初始化当前用户配置
1 执行此命令前，请一定要谨慎！请一定要明白你在做什么！
2 rm -r ~/.*
3 重启。
11.18 初始化 root 用户配置
1 执行此命令前，请一定要谨慎！请一定要明白你在做什么！
2 sudo rm -r /root
3 重启。
11.19 查询命令软链接
1 例如：ls -l $(which gcc)
2 显示：lrwxrwxrwx 1 root root 5 9月 17 22:14 /usr/bin/gcc -> gcc-6
11.20 top 命令技巧
1 top是一个常见的进程查看命令，在top运行界面按下h可查看帮助。
2 按下1:查看各CPU占用率。
3 按下m:查看内存使用情况。
4 按下c:查看命令详细路径。
5 按下L：搜索进程。
11.21 查看指定行的内容
1 查看第3行至第5行共3行：sed -n 3,5p /etc/default/grub
2 查看第3行和第5行共2行：sed -n "3p;5p" /etc/default/grub
Deepin UOS 深度技术群：19346666 65
11.22 搜索匹配多个关键词 第十一章 DEEPIN 终端操作技巧集锦
11.22 搜索匹配多个关键词
1 区分大小写：lspci |grep -E "VGA|3D"
2 不区分大小写：lspci |grep -Ei "vga|3d"
11.23 字符串截取
1 以str变量为例：str=gmp-6.1.0.tar.bz2
2 echo ${str} |cut -d '-' -f 1 #以‘-’分隔，输出第1列gmp
3 echo ${str%%-*} #以‘-’分隔，最大限度从前面截取字符串gmp
4 echo ${str##*.} #以‘.’分隔，最大限度从后面截取字符串bz2
5 echo ${str:0:3} #从左开始输出3个字符gmp
6 echo ${str:4} #从左面第5个字符开始输出直到结束6.1.0.tar.bz2
7 echo ${str:4:5} #从第5个字符开始输出5个字符6.1.0
8 echo ${str:0-8} #从右开始输出8个字符.tar.bz2
Deepin UOS 深度技术群：19346666 66
第十二章 ArchLinux DDE 折腾笔记
12.1 下载 Arch 安装镜像，阅读安装指南
1 ArchLinux中的DDE更新十分频繁，可以看作是DDE的内部测试版。本章节尝试总结Arch中安装
DDE的最简步骤，且只支持UEFI+GPT方式，只推荐给因电脑太新，导致无法安装Deepin却
又十分喜欢DDE桌面的用户。
2 官方问题反馈地址：https://github.com/linuxdeepin/developer-center/issues
3 注意：Arch不适合新手，也不适合自学能力差的用户。
4 镜像下载地址：https://mirrors.tuna.tsinghua.edu.cn/archlinux/iso/latest/
5 官方安装维基：https://wiki.archlinux.org/index.php/Installation_guide
6 中文论坛安装：https://bbs.archlinuxcn.org/viewtopic.php?id=1037
7 知乎安装指南：https://www.zhihu.com/question/21427410
12.2 安装 1：连接网络
1 有线网络自动获取地址：安装前插好网线，或者手动执行dhcpcd
2 无线网络：wifi-menu
3 如提示“No networks found”，执行 rfkill unblock wifi 后再次：wifi-menu
4 ip link 或 iw dev 查询接口，lspci -k |more 查询驱动。
5 详见：https://wiki.archlinux.org/index.php/Network_configuration/
Wireless ，可切换至中文语言查看。
12.3 安装 2：分区与挂载
1 分区：fdisk结合cfdisk，磁盘GPT分区格式，必须创建一个EFI分区，lsblk或parted -l可
查看详情。这里仅以一个必备的EFI分区和一个必备的根分区举例。
2 格式化示例：
3 mkfs.fat -F32 /dev/sda1
4 mkfs.ext4 /dev/sda2
5 挂载示例：
6 mount /dev/sda2 /mnt
7 mkdir -p /mnt/boot/efi
8 mount /dev/sda1 /mnt/boot/efi
12.4 安装 3：换国内源
1 nano /etc/pacman.d/mirrorlist
2 Ctrl+W搜索tuna，Ctrl+K剪切，Ctrl+HOME跳到第一行，Ctrl+U把清华大学的源优先级调到
最高。继续搜索ustc，同样的方法把中科大的源放在第二优先级。
3 Ctrl+O保存，Ctrl+X退出。
67
12.5 安装 4：安装与配置 第十二章 ARCHLINUX DDE 折腾笔记
12.5 安装 4：安装与配置
1 注意：以下步骤只适用UEFI+GPT磁盘格式，BIOS+MBR已经过时了。为了提高稳定性，默认安装
LTS内核。请严格按步骤操作，相关知识欠缺的，请阅读官方维基补充。
2 安装：pacstrap /mnt base linux-lts linux-firmware grub efibootmgr os?prober sudo nano networkmanager deepin deepin-extra
3 自动挂载：genfstab -U /mnt >> /mnt/etc/fstab
4 切换系统：arch-chroot /mnt
5 系统引导：grub-install && grub-mkconfig -o /boot/grub/grub.cfg
6 启用桌面：systemctl enable lightdm
7 启用网络：systemctl enable NetworkManager
8 创建用户：useradd -m -G wheel <用户名>
9 修改密码：passwd <用户名>
10 授予权限：nano /etc/sudoers，取消 %wheel ALL=(ALL) ALL 所在行的注释。
11 退出系统：exit
12 卸载重启：umount -R /mnt && reboot
12.6 安装 5：后期批处理
1 将以下内容保存为arch-dde-setup.sh，登陆DDE后给予可执行权限并在终端运行。
2 #! /bin/bash
3 # 主机名
4 read -p "Please input the hostname: " hostname
5 sudo hostnamectl set-hostname $hostname
6 sudo bash -c 'echo -e "\n127.0.0.1\thostname\n127.0.0.1\t$hostname" >>
/etc/hosts'
7 # 时区
8 sudo timedatectl set-timezone Asia/Shanghai
9 sudo timedatectl set-ntp true
10 sudo hwclock --localtime --systohc
11 # 中文
12 sudo bash -c 'echo -e "\nzh_CN.UTF-8 UTF-8\nen_US.UTF-8 UTF-8" >> /etc/
locale.gen'
13 sudo locale-gen
14 sudo localectl set-locale LANG=zh_CN.UTF-8
15 sudo pacman -S noto-fonts-cjk --noconfirm
16 # LTS内核头文件
17 sudo pacman -S linux-lts-headers --noconfirm
18 # 与LTS内核兼容
19 sudo pacman -S deepin-anything-dkms --noconfirm
20 # 软件源
21 sudo bash -c 'echo -e "\n[multilib]\nInclude = /etc/pacman.d/mirrorlist
" >> /etc/pacman.conf'
22 sudo bash -c 'echo -e "\n[archlinuxcn]\nServer = https://mirrors.tuna.
tsinghua.edu.cn/archlinuxcn/\$arch\nServer = https://mirrors.ustc.
edu.cn/archlinuxcn/\$arch" >> /etc/pacman.conf'
23 sudo pacman -Syy
Deepin UOS 深度技术群：19346666 68
第十二章 ARCHLINUX DDE 折腾笔记 12.7 使用 LTS 内核提高稳定性
24 sudo pacman -S archlinuxcn-keyring --noconfirm
25 # 常见软件
26 sudo pacman -S bash-completion --noconfirm #终端自动完成
27 sudo pacman -S google-chrome --noconfirm #谷歌浏览器
28 sudo pacman -S deepin.com.qq.im deepin.com.qq.office --noconfirm #QQ
29 sudo pacman -S wps-office wps-office-mui-zh-cn ttf-wps-fonts --
noconfirm #WPS办公套装
30 sudo pacman -S visual-studio-code-bin --noconfirm #Visual Studio Code
31 sudo pacman -S netease-cloud-music --noconfirm #网易云音乐
32 sudo pacman -S neofetch --noconfirm #系统信息
33 sudo pacman -S gparted --noconfirm #分区管理器
34 sudo pacman -S gnome-disk-utility --noconfirm #磁盘
35 sudo pacman -S evince poppler-data --noconfirm #文档查看器
36 sudo pacman -S remmina --noconfirm #Windows远程桌面
37 sudo pacman -S vlc --noconfirm #视频播放器
38 sudo pacman -S audacious --noconfirm #音频播放器
39 sudo pacman -S git --noconfirm #版本管理
40 sudo pacman -S leafpad --noconfirm #文本编辑器
41 sudo pacman -S gnome-mines --noconfirm #扫雷
42 sudo pacman -S quadrapassel --noconfirm #俄罗斯方块
43 sudo pacman -S swell-foop --noconfirm #消色块
44 sudo pacman -S gnome-nibbles --noconfirm #贪吃蛇
45 # 禁用IPv6，修复QQ图片显示
46 sudo bash -c 'echo -e "net.ipv6.conf.all.disable_ipv6=1\nnet.ipv6.conf.
default.disable_ipv6=1" > /etc/sysctl.d/disable-ipv6.conf'
47 sudo sysctl -p /etc/sysctl.d/disable-ipv6.conf
48 # 输入法
49 sudo pacman -S fcitx-im fcitx-configtool --noconfirm
50 sudo pacman -S fcitx-skin-material --noconfirm
51 echo -e "export GTK_IM_MODULE=fcitx\nexport XMODIFIERS=@im=fcitx\
nexport QT_IM_MODULE=fcitx" > ~/.xprofile
52 read -p "Done. Press any key to reboot and enjoy." -n 1
53 reboot
54
55 该批处理脚本可从QQ群19346666群文件下载。
56 重启享用。
12.7 使用 LTS 内核提高稳定性
1 执行完上面五个步骤，说明Arch+DDE安装已经完成，并且通过第四步安装时选择“pacstrap /
mnt linux-lts”而不是“pacstrap /mnt linux”，默认安装的已经是LTS内核了。
2 所以下面内容只适合默认linux最新内核包的用户。
3 sudo pacman -S linux-lts linux-lts-headers --noconfirm
4 sudo pacman -Rdd linux linux-headers
5 sudo grub-mkconfig -o /boot/grub/grub.cfg
Deepin UOS 深度技术群：19346666 69
12.8 为 LTS 内核安装 DKMS 后缀包 第十二章 ARCHLINUX DDE 折腾笔记
12.8 为 LTS 内核安装 dkms 后缀包
1 对于LTS内核和定制内核，建议安装后缀名为dkms的包，可以获得更好的稳定性。
2 如果你发现Arch+DDE卡顿，建议尝试：
3 sudo pacman -S deepin-anything-dkms
12.9 安装 NVIDIA 显卡驱动
1 LTS内核需安装：sudo pacman -S nvidia-lts
2 非LTS内核安装：sudo pacman -S nvidia
3 详见：https://wiki.archlinux.org/index.php/NVIDIA
4 双显卡用户还需：sudo pacman -S bbswitch-dkms optimus-manager-qt
5 重启后，在“Optimus管理器”设置Optimus切换方法为Bbswitch。
12.10 更多软件安装
1 sudo pacman -S qq-linux --noconfirm --needed #QQ For Linux
2 sudo pacman -S blender --noconfirm --needed #3D建模与视频剪辑
3 sudo pacman -S openshot --noconfirm --needed #视频剪辑
4 sudo pacman -S audacity --noconfirm --needed #音频编辑器
5 sudo pacman -S gimp --noconfirm --needed #图像处理
6 sudo pacman -S soundconverter --noconfirm --needed #音频转换器
7 sudo pacman -S simplescreenrecorder --noconfirm --needed #录屏
8 sudo pacman -S obs-studio --noconfirm --needed #录屏
9 sudo pacman -S filezilla --noconfirm --needed #FTP客户端
10 sudo pacman -S clang gcc gdb cmake ninja --noconfirm --needed #开发
12.11 pacman 常见用法
1 维基文档：https://wiki.archlinux.org/index.php/Pacman
2 安装：sudo pacman -S package_name1 package_name2 ...
3 卸载但保留依赖：sudo pacman -R package_name
4 连同依赖一起卸载：sudo pacman -Rs package_name
5 升级整个系统：sudo pacman -Syu
6 从数据库查询软件包：pacman -Ss string1 string2 ...
7 查询本地安装的包：pacman -Qs string1 string2 ...
8 安装本地包：sudo pacman -U /path/to/package_name-version.pkg.tar.xz
9 查询已安装软件包文件列表：pacman -Ql package_name
10 查询未安装软件包文件列表：pacman -Fl package_name
11 按文件名查找软件包：pacman -F string1 string2 ...
12 清除未安装软件包的缓存：sudo pacman -Sc
13 清理所有软件包缓存：pacman -Scc
Deepin UOS 深度技术群：19346666 70
第十二章 ARCHLINUX DDE 折腾笔记 12.12 清除孤儿包
12.12 清除孤儿包
1 查询孤儿包：pacman -Qdt
2 查询孤儿包且不显示版本号：pacman -Qdtq
3 卸载孤儿包：sudo pacman -Rs $(pacman -Qdtq)
4 或者：pacman -Qdtq |pacman -Rs -
12.13 yay 替代 pacman
1 先安装yay：sudo pacman -S yay
2 yay提供原生pacman支持，在具备pacman几乎所有功能的基础上，还支持AUR软件安装。
3 例如安装微信：yay -S deepin.com.wechat2
4 安装QQ轻聊版：yay -S deepin.com.qq.im.light
5 搜索并选择安装示例：yay wechat
6 相对pacman六个字母而言，更喜欢三个字母的apt。
7 好在yay也是三个字母了^_^
12.14 yay 扩展用法
1 查询软件包信息：yay -Ps
2 卸载不需要的依赖包：yay -Yc
12.15 yay 缓存路径
1 yay编译安装AUR软件的缓存路径在：~/.cache/yay
2 当出现源码或者补丁下载失败时，可以手动下载后拷贝到相应目录。
3 当编译成功后，也可以拷贝pkg.tar.xz安装包备用。
12.16 免密码挂载分区
1 文件管理器挂载非系统分区时需要密码验证，非常麻烦。解决办法：
2 sudo nano /usr/share/polkit-1/actions/org.freedesktop.UDisks2.policy
3 修改filesystem-mount-system的allow_active值为yes即可免密。
4 <action id="org.freedesktop.udisks2.filesystem-mount-system">
5 ...
6 <defaults>
7 <allow_any>auth_admin</allow_any>
8 <allow_inactive>auth_admin</allow_inactive>
9 <allow_active>yes</allow_active>
10 </defaults>
11 </action>
Deepin UOS 深度技术群：19346666 71
12.17 备用 NEMO 文件管理器 第十二章 ARCHLINUX DDE 折腾笔记
12.17 备用 Nemo 文件管理器
1 yay -S nemo nemo-fileroller nemo-share nemo-preview cinnamon?translations gnome-terminal
2 DDE文件管理器不是很稳定，可以把Nemo当作备用。
12.18 KWin 无法开启窗口特效
1 删除：~/.config/kwinrc，重启。
12.19 外部磁盘挂载改/media/$USER
1 ArchLinux默认会把外部磁盘和可移动磁盘挂载在/run/media/$USER/目录，和别的发行版不
同，当多系统共享数据分区时，会带来环境变量配置上的不便。建议软链接可解决：
2 创建/media文件夹：sudo mkdir /media
3 创建软件链接：sudo ln -s /run/media/$USER /media/$USER
12.20 删除不再需要的软件
1 在想卸载的软件包上单击右键选择“发送桌面”，用编辑器打开该软件桌面启动器，找到“Exec
=/path/to/executeble”，然后用pacman -F /path/to/executeble查找软件包即
可定位后卸载。
12.21 禁止无密码授权
1 如果打开“分区编辑器”这类需要密码授权的应用，不输入密码或者随意输入密码就可以通过认
证，则首先确定用户是否在wheel组中：groups <用户名>
2 如果用户不在wheel组，则添加：sudo gpasswd -a <用户名> wheel
3 删除用户组示例：sudo gpasswd -d <用户名> <组名>
12.22 禁止 root 用户登陆
1 禁止登陆：sudo passwd -l root
2 解除锁定：
3 sudo nano /etc/shadow
4 将第一行root:!:<数字>::::::中的!删除，变成root::<数字>::::::
5 保存退出。
Deepin UOS 深度技术群：19346666 72
第十三章 Debian 10 折腾笔记
13.1 自定义安装 GNOME 桌面
1 为了实现wifi联网安装，请从清华大学镜像站下载集成非自由硬件驱动的网络安装镜像：
2 地址：https://mirrors.tuna.tsinghua.edu.cn/debian-nonfree/cd-including?firmware/current/amd64/iso-cd/firmware-10.3.0-amd64-netinst.iso
3 也可以下载集成非自由硬件驱动的标准版LIVE镜像：
4 https://mirrors.tuna.tsinghua.edu.cn/debian-nonfree/cd-including?firmware/current-live/amd64/iso-hybrid/debian-live-10.3.0-amd64-
standard+nonfree.iso
5 如果需要连接wifi安装，需要在配置网络时，把无线网卡作为主网络接口。
6 建议选择中国mirrors.huaweicloud.com镜像源，网络安装镜像需要在“软件选择”界面用空
格键取消“Debian 桌面环境”的选择，否则默认会安装GNOME桌面。
7 网络安装镜像相对LIVE镜像，安装速度要慢一些。
8 安装完成后重启进入终端，登陆设置LANG=C环境变量，可避免中文乱码。
9 终端wifi连接见下一条讲解。
10 sudo nano /etc/apt/source.list，删除security.debian.org源。
11 更新：sudo apt update
12 桌面：sudo apt install gnome-core
13 字体：sudo apt install fonts-noto-cjk
13.2 Debian Shell 连接 wifi
1 以下命令需要root权限：sudo -i
2 查看接口：iw dev
3 启用接口：ip link set wlan0 up
4 连接网络：wpa_supplicant -B -i wlan0 -c <(wpa_passphrase SSID PASSWORD)
5 获取地址：dhclient wlan0
6 如果提示：Operation not possible due to RF-kill，则需要下载rfkill包解锁：
https://packages.debian.org/buster/utils/rfkill
7 拷贝到U盘后mount到/mnt，dpkg -i离线安装，然后执行：rfkill unblock wifi
8 再次执行ip link set wlan0 up即可启用。
13.3 更换国内软件源
1 应用程序中运行“Software & Updates”：
2 1. Debian Software页面勾选“带有非自由依赖关系的DFSG兼容软件(contrib)”、“非
DFSG兼容软件(non-free)”和“源代码”，“下载自”选择“Other...”，在中国服务
器中选择“mirrors.huaweicloud.com”。
3 2. Updates页面去掉“安全更新(*/updates）”，否则速度奇慢！
4 关闭，重新载入。
73
13.4 终端命令自动完成 第十三章 DEBIAN 10 折腾笔记
13.4 终端命令自动完成
1 sudo apt install bash-completion
2 注销或重启生效。
13.5 驱动无线网卡
1 lspci |grep Network #查看厂商
2 多数：sudo apt install firmware-realtek
3 或者：sudo apt install firmware-iwlwifi
4 少数：sudo apt install firmware-ralink
5 根据无线网线型号，安装后重启生效。
13.6 驱动 Nvidia 显卡
1 如果你发现Debian非常卡顿迟缓，这说明没有正确安装显卡驱动。
2 sudo apt install nvidia-driver
3 重启生效。
13.7 安装中州韵 rime-ibus 输入法
1 安装ibus-rime: sudo apt install ibus-rime
2 “设置-Region & Language - 输入源”，添加“汉语(RIME)”。
3 单击托盘输入法图标部署，Ctrl+`或F4选择输入法方案和输入选项切换。
4 下载配置、词库：https://www.github.com/loaden/rime
5 覆盖到 ~/.config/ibus/rime 目录下，托盘输入法图标左键单击菜单“部署”。
13.8 为终端设置 Ctrl+Alt+T 快捷键
1 WIN+A打开设置，设备-Keyboard-键盘快捷键，在页面底端点击+号添加gnome-terminal命
令的快捷键，名称随意。
13.9 启用触摸板轻拍以点击
1 WIN+A打开设置，设备-Mouse & Touchpad-触摸板，启用“轻拍以点击”。
13.10 启用触摸板双指滚动
1 WIN+A打开设置，设备-Mouse & Touchpad-触摸板，启用“双指滚动”和“自然滚动”。
Deepin UOS 深度技术群：19346666 74
第十三章 DEBIAN 10 折腾笔记 13.11 重启 GNOME SHELL
13.11 重启 GNOME Shell
1 Alt+F2，输入r回车。
13.12 启用 macOS 风格桌面
1 应用程序搜索“Dash”，在搜索结果中点击“软件”分类，安装“Dash to Dock”扩展，从扩
展设置中将Dock显示在底部，根据喜好调整设置。
2 建议从源里安装：sudo apt install gnome-shell-extension-dashtodock
3 Alt+F2输入r启动Shell后，在“优化”程序中启用扩展，点击齿轮图标视喜好配置。
13.13 启用 Windows 风格桌面
1 应用程序搜索“Dash”，在搜索结果中点击“软件”分类，安装“Dash to Panel”扩展。
2 建议从源里安装：sudo apt install gnome-shell-extension-dash-to-panel
3 启动“优化”程序，在窗口标题栏页面启用“最大化”和“最小化”按钮。
13.14 NetworkManager 托管网络
1 sudo nano /etc/NetworkManager/NetworkManager.conf
2 设置：managed=true
3 重启：sudo systemctl restart NetworkManager
13.15 显示托盘图标
1 应用程序搜索“Tray”，在搜索结果中点击“软件”分类，安装“Tray Icons”扩展。
13.16 免密码挂载分区
详见12.16
13.17 Backport 软件安装
1 参考网址：http://backports.debian.org/Instructions/
2 终端执行：sudo nano /etc/apt/sources.list.d/backports.list
3 添加内容：deb http://deb.debian.org/debian buster-backports main
4 安装方法：sudo apt -t buster-backports install "package"
5 更新列表：http://backports.debian.org/changes/buster-backports.html
Deepin UOS 深度技术群：19346666 75
13.18 DEBIAN 急救模式修复 GRUB 引导 第十三章 DEBIAN 10 折腾笔记
13.18 Debian 急救模式修复 GRUB 引导
1 下载Debian网络安装镜像制作USB启动盘，Advanced options > Rescue mode进入急救模
式，可跳过网络配置和较时步骤。
2 方法一：急救模式菜单，选择：重新安装GRUB启动引导器
3 方法二：急救模式菜单，选择：在/dev/sdaX根分区中运行shell，然后执行grub-install
Deepin UOS 深度技术群：19346666 76
第十四章 Ubuntu 18.04 LTS 折腾笔记
14.1 Ubuntu 最小化安装
1 建议安装时选择“最小安装”以及“为图形或无线硬件，以及其它媒体格式安装第三方软件”。
2 Ubuntu在有网络连接的情况下，安装时无法指定国内源，有可能出现网络下载缓慢现象。此时可
以点击右侧“跳过”取消网络下载更新。
3 如果无法跳过下载，可以拔掉网线或者切断无线连接，安装完成后换国内源再更新。
14.2 更换国内软件源
1 应用程序中运行“软件和更新”：
2 1. “Ubuntu 软件”页面“下载自”选择“其他站点...”，在中国服务器中选择“mirrors.
tuna.tsinghua.edu.cn”。
3 2. “更新”页面取消勾选“重要安全更性(*-security)”，因为源的速度太慢。选择清华源
后，请先取消“推荐更新(*-updates)”和“不支持的更新(*-backports)”，再选中，
就改用国内源了，大幅度加快更新速度。这两个源不要取消，否则部分软件无法安装。
4 3. “开发者选项”页面取消勾选“提前释放出的更新”。
14.3 驱动独立显卡
1 应用程序中运行“软件和更新”，在“附加驱动”页面选择专用驱动并应用更改。
2 如果该页面为空，可能需要更新系统后重启再试。
14.4 禁用 GNOME 软件的 Snap 插件
1 启用Snap插件的Ubuntu软件安装速度在国内太慢了，建议卸载：
2 sudo apt purge gnome-software-plugin-snap
14.5 安装优化程序
1 最小化安装的Ubuntu，默认没有优化程序，可自行安装。
2 sudo apt install gnome-tweaks
14.6 界面设置与优化
1 应用程序搜索“Dash”，在搜索结果中点击左侧“Ubuntu软件”分类，安装“Dash to Dock
”，根据喜好配置。
2 如果在软件界面安装困难，可以从源中安装，重启Shell后通过“优化”程序启用：
3 sudo apt install gnome-shell-extension-dashtodock
77
14.7 添加五笔输入法 第十四章 UBUNTU 18.04 LTS 折腾笔记
14.7 添加五笔输入法
1 设置－区域和语言－输入源，点击＋号添加“汉语（极点五笔）”。
2 选中该输入法，点击齿轮图标设置横向和5个候选。
14.8 添加与卸载 PPA 源
1 添加：
2 sudo add-apt-repository ppa:XXX/YYY
3 sudo apt update
4 sudo apt install YYY
5 卸载：
6 sudo apt install ppa-purge
7 sudo ppa-purge ppa:XXX
Deepin UOS 深度技术群：19346666 78
第十五章 更多笔记·部分已过时
15.1 LightDM 配置维护
15.1.1 修改 lightdm 登陆分辨率
1 查询：xrandr -q
2 输出：HDMI-0 connected primary 1920x1080+0+0 (normal...
3 测试：xrandr --output HDMI-0 --primary --mode 1920x1080
4 修改：sudo nano /etc/lightdm/lightdm.conf
5 添加：display-setup-script=xrandr --output HDMI-0 --primary --mode 1920
x1080
15.1.2 解决 lightdm 不加载.profile
1 将~/.profile复制为~/.bash_profile
2 新建：~/.xsessionrc，添加内容：
3 if [ -f ~/.bash_profile ]; then
4 . ~/.bash_profile
5 fi
15.1.3 lightdm 用户自动登陆
1 sudo nano /etc/lightdm/lightdm.conf
2 修改：autologin-user=<用户名>
15.2 屏幕亮度修正
15.2.1 方法一
1 查询最大亮度：cat /sys/class/backlight/acpi_video0/max_brightness
2 sudo apt install gnome-settings-daemon
3 sudo nano /usr/bin/bright
4 添加：
5 #!/bin/bash
6 pkexec /usr/lib/gnome-settings-daemon/gsd-backlight-helper --set?brightness 15
7 其中--set-brightness 15中的值视需要在max_brightness的1/2和3/4之间取。
8 添加可执行权限：chmod +x /usr/bin/bright
9 设置：
10 sudo apt install libglib2.0-bin
11 gsettings set org.gnome.settings-daemon.peripherals.input-devices
hotplug-command "/usr/bin/bright"
12 查看：
13 cat /sys/class/backlight/acpi_video0/*brightness
79
15.3 创建 ANDROID 可连接的 WIFI 热点 第十五章 更多笔记·部分已过时
15.2.2 方法二
1 sudo apt install xbacklight
2 编辑：~/.profile
3 添加：xbacklight -set 60
15.3 创建 Android 可连接的 WIFI 热点
1 查看无线网上型号，确定驱动：sudo lshw -class network
2 例如：“vendor: Ralink”
3 则需要安装驱动：sudo apt install firmware-ralink
4 否则网卡会处在禁用状态：*-usb:1 DISABLED
5 sudo apt install hostapd
6 sudo nano /etc/default/hostapd
7 添加：DAEMON_CONF="/etc/hostapd/hostapd.conf"
8 sudo nano /etc/hostapd/hostapd.conf
9 添加：
10 interface=wlan0
11 bridge=br0
12 driver=nl80211
13 ssid=Forever
14 hw_mode=g
15 channel=6
16 macaddr_acl=0
17 auth_algs=1
18 wpa=3
19 wpa_passphrase=20070831
20 wpa_key_mgmt=WPA-PSK
21 wpa_pairwise=TKIP
22 rsn_pairwise=CCMP
23 桥接：apt install bridge-utils
24 sudo nano /etc/network/interfaces
25 添加：
26 # loopback network interface
27 auto lo br0
28 iface lo inet loopback
29 # wireless wlan0
30 allow-hotplug wlan0
31 iface wlan0 inet manual
32 # eth0 connected to the ISP router
33 allow-hotplug eth0
34 iface eth0 inet manual
35 # setup bridge
36 iface br0 inet static
37 bridge_ports wlan0 eth0
38 address 192.168.5.195
39 netmask 255.255.255.0
Deepin UOS 深度技术群：19346666 80
第十五章 更多笔记·部分已过时 15.4 WINE 配置方法
40 gateway 192.168.5.253
41 dns-nameservers 192.168.5.253 8.8.8.8 8.8.4.4
15.4 Wine 配置方法
15.4.1 配置 Wine 纯净版
1 1. Dash -> 搜索wine，运行Configure Wine配置程序
2 2. 激活“函数库”页面，在“新增函数库顶替”下拉框里输入“winemenubuilder.exe”，
添加，编辑，停用
3 3. 激活“函数库”页面，在“新增函数库顶替”下拉框里输入“winemine.exe”，添加，编
辑，停用
4 如果已经将int main() { return 0; }编译成main.exe，则可以执行：
5 cp -f main.exe $HOME/.wine/drive_c/windows/system32/winemenubuilder.exe
6 cp -f main.exe $HOME/.wine/drive_c/windows/system32/winemine.exe
7 然后将第2、3两步中的停用改成原装。
8 4. “驱动器”页面，添加D分区，路径指定为$HOME/qpSOFT/Wine；同时将Z分区路径修改为
$HOME
9 5. “关于”页面，填写Windows注册信息，姓名：loaden，单位：qpsoft
10 6. 运行Winetricks程序，安装字体：corefonts，然后从XP系统拷贝simhei.ttf simsun
.ttc至Fonts目录
11 7. 视需要安装DLL或组件：winetricks cmd vcrun6
15.4.2 彻底清理 Wine
1 删除$HOME/.local/share/applications/mimeapps.list中含有wine的条目
2 删除$HOME/.wine目录
3 find $HOME/.config -name '*wine*' -exec rm {} \;
4 find $HOME/.local -name '*wine*' -exec rm {} \;
5 find $HOME/.local -name '*wine*' -exec rm -r {} \;
6 rm -rf $HOME/.local/share/icons/hicolor
7 rm -f $HOME/.local/share/applications/mimeinfo.cache
15.4.3 Wine 调用批处理时字体错误处理
1 err:wineconsole:WCUSER_SetFont wrong font
2 err:wineconsole:WINECON_Fatal Couldn't find a decent font, aborting
3 '推荐方案：
4 $wine cmd
5 $XXX.bat
6 备用方案：
7 $LANG=C
8 $wineconsole cmd 或$wineconsole XXX.bat
9 这样就不会存在找不到中文字体的问题了，但要支持中文：
10 1. 批处理文件编码必须是GBK
11 2. 行尾必须用Windows风格
Deepin UOS 深度技术群：19346666 81
15.5 MLDONKEY 选项设置 第十五章 更多笔记·部分已过时
15.4.4 64 位系统，通过 Wine 模拟纯 32 位 Windows
1 打开终端，预设环境变量：
2 export WINEARCH=win32
3 export WINEPREFIX=$HOME/.wine32/
4 winecfg
5 winetricks ie6
6 这样就可以解决64位中，Wine无法安装32位IE的错误。
7 不过以后每次运行纯32位Windows中的程序，例如IE6，就需要先导出环境变量了。
8 通过bash脚本可以简化操作：wine32.sh
9 #!/bin/bash
10 export WINEARCH=win32
11 export WINEPREFIX=$HOME/.wine32/
12 winefile
13 在文件管理器中双击安装或运行。
15.4.5 英文系统安装 Wine 及中文支持
1 sudo apt install wine winetricks #wine
2 Alt+F2运行wine，按弹出提示操作，之后配置。
3 英文环境中文乱码：
4 单个程序：LANG="zh_CN.UTF8" wine XXX.exe
5 所有程序：修改/usr/bin/wine
6 改最后一行：exec "$WINELOADER" "$@"
7 为：LANG=zh_CN.UTF8 exec "$WINELOADER" "$@"
8 注意：如果安装程序时出现崩溃，考虑先还原这一行，安装完成后再恢复。
15.5 MlDonkey 选项设置
1 Options > Web infos，Remove掉所有项目，清空~/.mldonkey/web_infos目录后添加下
面三项：
2 server.met http://ed2k.im/server.met 24
3 guarding.p2p http://ed2k.im/ipfilter.dat 96
4 kad http://ed2k.im/nodes.dat 24
5 Options > Client，修改：
6 max_hard_download_rate 0
7 max_opened_connections 600
8 Options > Net，修改：
9 enable_kademlia true
10 enable_bittorrent false
11 enable_fileTP false
12 外网用户或者启用了UPnP，还可以：
13 ED2K-force_client_high_id true
14 ED2K-force_high_id true
15 局域网映射高ID：
16 apt install miniupnpc
17 在Help+ -> SysInfo里查port，然后添加到mlupnp脚本并复制到/usr/bin目录下：
Deepin UOS 深度技术群：19346666 82
第十五章 更多笔记·部分已过时 15.5 MLDONKEY 选项设置
18 #!/bin/bash
19 upnpc -r 18081 TCP 18085 UDP 8836 UDP && mlnet&
