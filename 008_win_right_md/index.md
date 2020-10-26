# Windows系统右键增加新建MrakDown


<!--more-->

## 一、保证已安装Typora



## 二、新建`.reg`文件并写入以下内容

```powershell
Windows Registry Editor Version 5.00
[HKEY_CLASSES_ROOT\.md]
@="Typora.exe"
[HKEY_CLASSES_ROOT\.md\ShellNew]
"NullFile"=""
[HKEY_CLASSES_ROOT\Typora.exe]
@="Markdown"
```

## 三、运行以上文件

以下为效果图

![右键添加MarkDown效果图](https://gitee.com/xiao_beita/tuchuang/raw/master/img/image-20201026132442346.png)

>   本文代码源自于[Windows下右键新建.md文件教程](https://stepneverstop.github.io/win-rightclick-create-md.html)
