# 下载与版本

请选择与你的电脑对应的安装包。Windows 与 Mac 分别维护版本号。

| 平台 | 系统要求 | 当前版本 | 下载 | 安装指南 |
| --- | --- | --- | --- | --- |
| Windows | Windows 10 / 11 x64，电脑微信 4.x | [v2.0](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/windows-v2.0) | [ZIP · 约 275 MiB](https://github.com/Leo-oo/wechat-ai-assistant/releases/download/windows-v2.0/Wechat-AI-Assistant-Windows-v2.0-20261025.zip) | [Windows 安装与使用](windows.md) |
| Mac | macOS 14+，Apple Silicon（M 系列） | [v2.4.2](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/macos-v2.4.2) | [DMG · 约 236 MiB](https://github.com/Leo-oo/wechat-ai-assistant/releases/download/macos-v2.4.2/AI.-Mac.v2.4.2-20261028.dmg) | [Mac 安装与使用](macos.md) |

Mac 版不支持 Intel 芯片。Windows 请完整解压后运行根目录的 **微信AI助手.exe**；Mac 请将 App 拖到“应用程序”后打开。

GitHub 自动提供的 **Source code (zip / tar.gz)** 是本说明仓库的快照，不是安装包。

## 文件校验

下载后可以计算 SHA256，与下表比较，确认文件完整性。校验一致不等于代码签名或安全审查。

| 下载文件 | 大小（字节） | SHA256 |
| --- | ---: | --- |
| `Wechat-AI-Assistant-Windows-v2.0-20261025.zip` | 288,137,692 | `d8c9820a961627404fe1ca2691dca191762b67a2e9f4258433c475407dd2895d` |
| `AI.-Mac.v2.4.2-20261028.dmg` | 247,861,734 | `bba80d0accd16fe326effe84459750dfd41141cdcb8201c031c487e5be8baac7` |

Windows 在下载目录打开 PowerShell：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\Wechat-AI-Assistant-Windows-v2.0-20261025.zip'
```

Mac 在下载目录打开终端：

```sh
shasum -a 256 'AI.-Mac.v2.4.2-20261028.dmg'
```

Windows v2.0 的 Release 同时提供同名 `.sha256` 校验文件，对应当前英文附件名，无需改名。Mac v2.4.2 请使用上面的命令与表中 SHA256 比较；不要用旧版本的校验文件检查新安装包。

## 版本说明

- [Windows v2.0](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/windows-v2.0)
- [Mac v2.4.2](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/macos-v2.4.2)


Windows 程序尚未代码签名；Mac App 使用 ad-hoc 签名，未经过 Apple 开发者签名和公证。遇到系统阻止打开时，请保留完整提示并参考安装指南，不要关闭系统安全保护。
