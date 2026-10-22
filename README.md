# Codex Pocket Bridge Releases

Codex Pocket 的 macOS 与 Windows 桌面 Bridge 正式安装包仓库。

当前正式版本：[0.10.19](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/tag/v0.10.19)，同步聊天历史分页、iOS 安全读取的 TLS 连接复用及 Windows 启动修复。

| 平台 | 下载与状态 |
| --- | --- |
| Windows 11 x64 | [0.10.19 正式安装包](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.19/PocketBridge-0.10.19-Windows-x64.zip)，完整解压后运行 `Install-PocketBridge.cmd`；当前用户脚本安装包，内含运行时，无需管理员权限 |
| macOS Apple Silicon，macOS 14+ | [0.10.19 ARM 安装包](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.19/PocketBridge-0.10.19-arm64.pkg)，已在 Apple Silicon Mac 覆盖安装并与 iPhone 验证连接 |
| macOS Intel，macOS 13+ | [此前 0.10.10 Intel 安装包](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.10/PocketBridge-0.10.10-x86_64.pkg)，本轮没有 0.10.19 Intel 包，真实 Intel 硬件尚未验证 |

安装前先在电脑安装并登录 Codex，在手机和电脑开启 Tailscale，并允许两端互访。电脑需要保持唤醒和联网。首次使用时打开 Bridge，点击“添加手机”，用 Pocket 扫码并在电脑核对确认码、允许连接。覆盖升级前等待运行中的任务结束，已有配对记录保留，无需先卸载。

Windows 0.10.19 已通过 29 项跨平台回归检查和最终安装包完整性校验；2 项原生 Windows 检查跳过。尚未在真实 Windows 上验证安装、自启、窗口/托盘与控制台关闭后的进程存活，详细验证范围见版本说明。

Mac 应用使用 ad hoc 签名，安装包尚未完成 Developer ID 签名与公证。首次安装可能需要在系统设置 → 隐私与安全性中单独放行。

[校验文件 SHA256SUMS](https://github.com/lorinDev/CodexPocketBridgeReleases/releases/download/v0.10.19/SHA256SUMS)。Android APK 与 Build CLI 更新目录继续位于独立的 [CodexPocketReleases](https://github.com/lorinDev/CodexPocketReleases/releases) 仓库；本仓库不发布 iOS 安装包。
