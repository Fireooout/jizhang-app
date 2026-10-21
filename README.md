# 项目记账 · Android App

[项目记账](https://jz.plaseco.tech) 的安卓客户端，基于 Capacitor 6 封装，直接加载 https://jz.plaseco.tech，网页更新后 App 自动同步。

- 包名：`tech.plaseco.jz`
- 原生功能：附件/报表下载（系统下载管理器，保存到「下载/项目记账」）、拍照上传、返回键后退、断网提示
- 编译：推送到 `main` 分支后，GitHub Actions 会自动编译签名版 APK，在 Actions → 本次运行 → Artifacts 中下载
- 签名：`signing/release.jks.enc` 是经过 AES-256 加密的签名证书，编译时用仓库 Secret `KEYSTORE_PASSWORD` 解密
