# 命令行激活Windows系统和Office


**使用命令行激活 Windows 系统和 Office**

<!--more-->

## 1. kms激活Windows系统，(推荐数字激活)

```cmd
# 以管理员权限的CMD或PowerShell运行以下命令
slmgr /skms kms.v0v.bid
slmgr /ato
```

---

---

## 2. 激活默认安装的64位Office：适用于批量版的2010;2013;2016;2019

```cmd
# 以管理员权限的CMD或PowerShell运行以下命令
cd "C:\Program Files\Microsoft Office\Office*"
cscript ospp.vbs /sethst:kms.v0v.bid
cscript ospp.vbs /act
```

---

---

## 3. 想法来源和安装Office地址

> [Windows系统一句命令激活](https://v0v.bid/kms.html)

> [Office Tool Plus](https://otp.landian.vip) 注：部署批量版


