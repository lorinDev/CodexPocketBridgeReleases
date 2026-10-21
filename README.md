# Codex Pocket Bridge Releases

Codex Pocket 的桌面 Bridge 安装包仓库，面向 macOS 和后续 Windows 版本。

当前正式版本：[0.10.2](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/tag/v0.10.2)。

| 平台 | 下载与状态 |
| --- | --- |
| macOS Apple Silicon，macOS 14+ | [ARM 安装包](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.2/PocketBridge-0.10.2-arm64.pkg) |
| macOS Intel，macOS 13+ | [Intel 安装包](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.2/PocketBridge-0.10.2-x86_64.pkg)，当前以 Rosetta 验证，真实 Intel 硬件待验收 |
| Windows 11 x64 | [连接验证启动工具](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.2/PocketBridge-Windows-x64-Connection.zip)；实际运行验证中，正式安装器尚未发布 |

安装前先在电脑安装并登录 Codex，在手机和电脑开启 Tailscale，并允许两端互访。打开 Bridge，点击“添加手机”，用 Pocket 扫码并在电脑核对确认码、允许连接。电脑需要保持唤醒和联网。

Mac 应用使用 ad hoc 签名，安装包尚未完成 Developer ID 签名与公证。真实手机蜂窝跨网连接仍待验收。

Android APK 与 Build CLI 更新目录继续位于独立的 [CodexPocketReleases](https://github.com/lorinDev/CodexPocketReleases/releases) 仓库。

2026-10-21：Windows 连接启动工具已更新到构建 2026-10-21.1，修复任务列表触发的 `CreateFile` 参数类型错误。升级前运行 `Stop-PocketBridge.cmd` 停止旧后台，再解压新包并运行 `Start-PocketBridge.cmd`；配对记录保留。实际 Windows 任务读取和桌面接续仍需用户电脑复验。
