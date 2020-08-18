# OpenWrt firmware for Newifi D2

Auto build OpenWrt firmware for Newifi D2 via GitHub Actions

[![GitHub release (latest by date)](https://img.shields.io/github/v/release/P3TERX/OpenWrt-Newifi_D2?style=for-the-badge&label=Download)](https://github.com/ZHDeveloper/OpenWrt-Newifi_D2/actions/)

### 开原驱动配置

```
CONFIG_PACKAGE_kmod-mt7603=y
CONFIG_PACKAGE_kmod-mt7603e=n
CONFIG_PACKAGE_kmod-mt76x2=y
CONFIG_PACKAGE_kmod-mt76x2-common=y
CONFIG_PACKAGE_kmod-mt76x2e=n
CONFIG_PACKAGE_wpad-openssl=y
CONFIG_PACKAGE_wpa-supplicant=y

CONFIG_PACKAGE_luci-app-mtwifi=n
```

### LuCI应用说明
[OpenWrt 编译 LuCI -> Applications 添加插件应用说明](https://www.right.com.cn/forum/thread-3682029-1-1.html)
