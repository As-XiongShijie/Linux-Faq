今天发现qt莫名奇妙的打不开了

修改配置文件~/.bashrc：

```
$ vim ~/.bashrc
```

在最末尾添加如下语句，会在qtcreator启动时，列出详细的错误提示。

```
export QT_DEBUG_PLUGINS=1
```

然后

![img](https://storage.deepin.org/thread/202104272055125805_截图_选择区域_20210427205500.png)

### **发现是少东西！ 可是我在安装之后是可以正常打开的啊？不知道为啥这个突然就没了！**

![img](https://storage.deepin.org/thread/202104272056147435_截图_选择区域_20210427205602.png)

调查之后发现问题出在QT 需要手动下载一个包安装之后才能解决。

![img](https://storage.deepin.org/thread/202104272057579683_截图_选择区域_20210427205719.png)

现在qt可以正常运行了

### 下载地址放这里了



https://packages.debian.org/bullseye/amd64/libxcb-util1/download



[作者]:XXTX



