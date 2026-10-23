# 下载与版本

请选择与你的电脑对应的安装包。Windows 与 Mac 分别维护版本号。

| 平台 | 系统要求 | 当前版本 | 下载 | 安装指南 |
| --- | --- | --- | --- | --- |
| Windows | Windows 10 / 11 x64，电脑微信 4.x | [v1.9](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/windows-v1.9) | [ZIP · 约 275 MiB](https://github.com/Leo-oo/wechat-ai-assistant/releases/download/windows-v1.9/AI.-Windows.v1.9-20261024.zip) | [Windows 安装与使用](windows.md) |
| Mac | macOS 14+，Apple Silicon（M 系列） | [v2.4.1](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/macos-v2.4.1) | [DMG · 约 236 MiB](https://github.com/Leo-oo/wechat-ai-assistant/releases/download/macos-v2.4.1/AI.-Mac.v2.4.1-20261023.dmg) | [Mac 安装与使用](macos.md) |

Mac 版不支持 Intel 芯片。Windows 请完整解压后运行根目录的 **微信AI助手.exe**；Mac 请将 App 拖到“应用程序”后打开。

GitHub 自动提供的 **Source code (zip / tar.gz)** 是本说明仓库的快照，不是安装包。

## 文件校验

下载后可以计算 SHA256，与下表比较，确认文件完整性。校验一致不等于代码签名或安全审查。

| 下载文件 | 大小（字节） | SHA256 |
| --- | ---: | --- |
| `AI.-Windows.v1.9-20261024.zip` | 288,129,892 | `a95cfc61fc6378654c6353eeae7cb1c8ddd7a57aaa6e134906dc649da850a2dc` |
| `AI.-Mac.v2.4.1-20261023.dmg` | 247,863,351 | `1e34a9a1e07b8bc9c83858aaa157b9cd8937160c66b16a02fbd8e87a0c6c0799` |

Windows 在下载目录打开 PowerShell：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\AI.-Windows.v1.9-20261024.zip'
```

Mac 在下载目录打开终端：

```sh
shasum -a 256 'AI.-Mac.v2.4.1-20261023.dmg'
```

Release 中的单文件 `.sha256` 保留了原始中文文件名。若使用它自动校验，请将文件分别改名为 `微信AI助手-Windows版v1.9-20261024.zip` 或 `微信AI助手-Mac版v2.4.1-20261023.dmg`；使用上面的命令直接比较哈希则无需改名。

## 版本说明

- [Windows v1.9：安装优化与示例查看](../release-notes/windows-v1.9.md)
- [Mac v2.4.1：安装与接入说明](../release-notes/macos-v2.4.1.md)

Windows 程序尚未代码签名；Mac App 使用 ad-hoc 签名，未经过 Apple 开发者签名和公证。遇到系统阻止打开时，请保留完整提示并参考安装指南，不要关闭系统安全保护。
