# 下载与版本

下面两个安装包与校验文件已上传到 GitHub Release 草稿，页面显示的安装包 SHA256 与本地原文件一致。仓库仍为私有，草稿尚未发布；只有具备相应草稿访问权限的成员可以检查，尚未开放公众下载。

- [查看 Windows v1.9 草稿](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/untagged-7fac9fdacdf0c15930c2)
- [查看 Mac v2.4.1 草稿](https://github.com/Leo-oo/wechat-ai-assistant/releases/tag/untagged-0a253cf363a30b70e430)

| 平台 | 版本 | 文件 | 精确大小 | 拟用 Release 标签 |
| --- | --- | --- | --- | --- |
| Windows | v1.9 | 微信AI助手-Windows版v1.9-20261024.zip | 288,129,892 字节 | `windows-v1.9` |
| Mac | v2.4.1 | 微信AI助手-Mac版v2.4.1-20261023.dmg | 247,863,351 字节 | `macos-v2.4.1` |

两个平台独立维护版本号。Windows 和 Mac 请分别选择对应 Release 的安装附件。

GitHub 上传时处理了中文文件名：当前 Windows 附件显示为 `AI.-Windows.v1.9-20261024.zip`，Mac 附件显示为 `AI.-Mac.v2.4.1-20261023.dmg`。这是文件名变化，安装包内容和校验值未改变。上表保留原始部署包名。使用随包的单文件 `.sha256` 校验时，可先将下载文件改回原始文件名；按下面命令直接计算哈希再比较时，不需要改名。

GitHub 自动生成的“Source code (zip)”和“Source code (tar.gz)”是本说明仓库的快照，不能用于安装程序。

## 文件校验

Windows ZIP 的 SHA256：

```text
a95cfc61fc6378654c6353eeae7cb1c8ddd7a57aaa6e134906dc649da850a2dc
```

Mac DMG 的 SHA256：

```text
1e34a9a1e07b8bc9c83858aaa157b9cd8937160c66b16a02fbd8e87a0c6c0799
```

哈希用于核对下载文件是否一致，不代表兼容性、代码签名或安全审查结论。

Windows 可在 PowerShell 执行：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\AI.-Windows.v1.9-20261024.zip'
```

Mac 可在终端执行：

```sh
shasum -a 256 'AI.-Mac.v2.4.1-20261023.dmg'
```

## 当前核验范围

Windows v1.9 已完成构建、文件清单和解压校验、隔离运行环境检查，以及 9 个桌面界面场景检查；上一轮自动测试 258 项通过、2 项跳过。尚未在另一台干净电脑完成首次真实接入验收。包内记录的第三方原生组件公开分发审查尚未完成。

Mac v2.4.1 本次仅核验文件名、大小及 SHA256；尚未在这台 Windows 电脑挂载或运行。支持的 macOS 版本、芯片架构、签名与安装步骤需要从 Mac 当前发行资料补齐。
