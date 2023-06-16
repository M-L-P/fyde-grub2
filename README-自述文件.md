[![GitHub release (latest by date)](https://img.shields.io/github/v/release/M-L-P/fyde-grub2)](https://github.com/M-L-P/fyde-grub2/releases/latest)
[![GitHub all releases](https://img.shields.io/github/downloads/M-L-P/fyde-grub2/total)](https://github.com/M-L-P/fyde-grub2/releases)
[![GitHub Discussions](https://img.shields.io/github/discussions/M-L-P/fyde-grub2)](https://github.com/M-L-P/fyde-grub2/discussions)
![GitHub Repo stars](https://img.shields.io/github/stars/M-L-P/fyde-grub2?style=social)

[English](README.md)|[简体中文](README-自述文件.md)|[繁體中文](README-繁體中文.md)|...
--|--|--|--

# fyde-grub2
这个是用来启动 fydeOS 的，添加了改编自 [brunch](https://github.com/sebanc/brunch) 的 grub 主题。
#### 文件结构树状图
<img src="https://raw.githubusercontent.com/M-L-P/.github/main/screenshots/fyde-grub2.png">

## 💻️预览👀

<details>
<summary>🖱️点击展开查看🖱️</summary>

![image](https://github.com/M-L-P/fyde-grub2/assets/69227436/c114e5bf-433c-4c11-8147-9630bb3cf5d6)<br/>
![image](https://github.com/M-L-P/fyde-grub2/assets/69227436/acaad98a-167b-4252-9279-004287719e56)
</details>

## 🧭指南⬇️

### 复制到 ESP
- 复制文件夹 `zip: ESP/EFI/fyde` 到 `ESP: \EFI`；

### 复制到 ext4
- 复制文件夹 `zip: ext4/boot/grub` 到 `FYDEOS-DUAL-BOOT: /boot`；
你可以在 fydeOS 上使用 crosh shell。
`Ctrl` + `Alt` + `t`
`shell`
```
sudo rm -rf /media/removable/FYDEOS-DUAL-BOOT/boot/grub/themes
cd ~/Downloads/ext4
sudo cp -f -r boot /media/removable/FYDEOS-DUAL-BOOT
sudo reboot
```

## 📝FAQ❓️
### 安全启动
- 我还没试过，但可能支持安全启动，如果你使用 `grub.cer`(安全启动证书)，
- - `grub.cer`(安全启动证书) 来自 [Ventoy](https://github.com/ventoy/Ventoy)；
### 启动入口菜单
- 我已经改编了 `grub.cfg` 使得那三个启动入口都变成通用的了，所以无论 `FYDEOS-DUAL-BOOT` 是哪个分区都能够启动。

## ⭐收藏🌟
如果你喜欢并且期待未来的更新，你可以点亮星星。💫

## 🎉来源🎊
- 绝大多数改编自 [Brunch Framework](https://github.com/sebanc/brunch);
- 安全证书来自 [Ventoy](https://github.com/ventoy/Ventoy);
- ...
