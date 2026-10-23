# Mac v2.4.1 · 2026-10-23

微信AI助手 Mac 版部署包。支持本机记录接入、交给 Agent 生成群日报 / 总结，并按需配置微信推送与定时摘要。

## 下载与安装

- [下载安装包（DMG · 约 236 MiB）](https://github.com/Leo-oo/wechat-ai-assistant/releases/download/macos-v2.4.1/AI.-Mac.v2.4.1-20261023.dmg)
- [Mac 安装与使用指南](https://github.com/Leo-oo/wechat-ai-assistant/blob/main/docs/macos.md)
- [完整 HTML 指南](https://github.com/Leo-oo/wechat-ai-assistant/blob/main/docs/macos-installation.html)

**需要 macOS 14 或更高版本、Apple Silicon（M 系列）芯片；不支持 Intel Mac。** 电脑微信应安装在 `/Applications/WeChat.app`。Python、Node 和基础运行环境已随包提供。

打开 DMG，将 **微信AI助手.app** 拖到“应用程序”，再从“应用程序”打开。首次使用先准备本机项目，再查看并确认接入计划。登录、扫码及系统授权需本人完成。

## 接入与使用

- 首次接入会创建独立微信副本并重新签名，临时获取本机解密凭证；不覆盖原微信 App，原聊天数据库只读。
- 凭证存入当前用户的 macOS 钥匙串；聊天解密缓存和报告保存在所选本机项目中。
- 接入完成后，复制群日报安装请求给能够访问本机文件的 Agent。生成 PNG 还需可用的 Chrome / Chromium / Edge。
- 微信推送、定时摘要和本地模型为可选配置，不会因安装 App 自动开启。
- 已有项目可在 App 中复用并检查升级；升级前备份，遇到自定义文件冲突先确认处理方式。

## 注意事项

App 使用 ad-hoc 签名，未经过 Apple 开发者签名和公证。若 macOS 阻止打开，请保留提示，不要直接移除隔离属性或关闭 Gatekeeper。

取消或失败后先检查状态与恢复提示，不连续重复接入。更新项目程序通常不需要重新取钥。

使用云端 Agent 整理时，所选范围的聊天素材会由该服务处理。钥匙串保护凭证，不代表解密缓存与报告已加密。

## 文件完整性

- 文件：`AI.-Mac.v2.4.1-20261023.dmg`
- 大小：247,863,351 字节。
- SHA256：`1e34a9a1e07b8bc9c83858aaa157b9cd8937160c66b16a02fbd8e87a0c6c0799`
