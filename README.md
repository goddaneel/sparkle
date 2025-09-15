# Sparkle-Lite
去除特权功能的 Sparkle 分支，测试中，可能存在恶性 Bug，请勿使用。

## 附属仓库
- [Sparkle Patch](https://github.com/goddaneel/sparkle-patch)
    包含一组基于 Bubblewrap 工具（仅适用于 GNU/Linux 平台）的测试构建沙盒。

## 修改日志
|修改内容|修改范围|产生影响|影响平台|上游版本|分支版本|
|-|-|-|-|-|-|
|修改版本号规则|修改 package.json 配置|与上游项目版本号规则有差异，不能混装|Linux x86|1.6.11|1.6.11-lite4|
|去除 mihomo 内核的 setuid 配置|修改 postinst 脚本|可能影响所有需要提权的内核功能（TUN、内置更新等）||||
|去除 chrome-sandbox 的 setuid 配置||可能影响旧版本 Electron 内置沙盒||||
|将 `productName` 从 `Sparkle` 改为 `sparkle`|修改 electron-builder.yml 配置|其他平台构建名称会发生改变||||