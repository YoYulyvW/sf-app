# SF App (iOS)

顺丰打印助手的 iOS 客户端，对接同仓库外部的 Go 后端（backend-go）HTTP API。

- 支持 iOS 15 / iOS 16
- 无签名，通过 TrollStore 安装
- 使用 GitHub Actions 自动构建 .ipa

## 本地开发

需要 macOS + Xcode + [XcodeGen](https://github.com/yonaskolb/XcodeGen)：

```bash
brew install xcodegen
xcodegen generate
open SFApp.xcodeproj
```

## 构建产物

推送到 main 分支后，GitHub Actions 会自动构建未签名 .ipa，在 Actions 运行记录的 Artifacts 里下载，用 TrollStore 安装。
