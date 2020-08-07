# scoop 使用教程


# 代码如下

```powershell
# 管理员运行powershell
# 设置powershell代理，只适用于v2ray,其他请修改相应端口
$Env:http_proxy="http://127.0.0.1:10809"
$Env:https_proxy="http://127.0.0.1:10809"

# 安装 scoop
Set-ExecutionPolicy RemoteSigned -scope CurrentUser
iwr -useb get.scoop.sh | iex
# 或
Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://get.scoop.sh')

scoop checkup                # 检查错误

# 安装
scoop install git sudo
sudo scoop install sudo -g

# 别名
scoop alias add as 'scoop update *|scoop cache rm *|scoop cleanup *' '更新清除'
scoop alias add l 'scoop list' '列表'

# 检查已添加的别名
scoop alias list -v

# 先添加bucket
scoop bucket add extras
scoop bucket add nirsoft
scoop bucket add dorado https://github.com/h404bi/dorado
scoop bucket add Ash258 'https://github.com/Ash258/Scoop-Ash258.git'
scoop bucket add nerd-fonts
scoop bucket add nonportable

# scoop 安装更纱字体
sudo scoop install SarasaGothic-SC -g

# scoop 安装软件
scoop install 7zip adb aria2 aria-ng-gui bilibili-livehime busybox clash-for-windows dark dismplusplus ffmpeg firefox git Hack-NF hugo-extended innounp jq lessmsi listary mobaxterm neatdownloadmanager nmap nodejs notepad3 officetoolplus pandoc python qtscrcpy rclone SarasaGothic-SC shadowsocksr-csharp Snipaste spacesniffer teamviewer trafficmonitor v2rayn vim vscode winscp
```


