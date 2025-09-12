# Sparkle-Lite
去除特权功能的 Sparkle 分支，测试中，可能存在恶性 Bug，请勿使用。

## 附属仓库
- [Sparkle Patch](https://github.com:goddaneel/sparkle-patch)
    包含一组基于 Bubblewrap 工具的测试构建沙盒。

## 此分支的修改
|修改内容|修改范围|产生影响|影响平台|上游版本|分支版本|
|-|-|-|-|-|-|
|去除 mihomo 内核的 setuid 权限|仅修改 postinst 脚本|可能影响所有需要提权的内核功能（tun、内核自更新等）|Linux|1.6.4|1.6.4+0.1|