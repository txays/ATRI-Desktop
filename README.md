# ATRI · My Dear Desktop

Windows 上的亚托莉桌宠：Live2D、表情、互动与衣橱，支持填写自己的模型服务进行文字聊天。

**[下载最新版](https://github.com/txays/ATRI-Desktop/releases/latest)** · **[全部历史版本](https://github.com/txays/ATRI-Desktop/releases)** · **[使用说明](https://github.com/txays/ATRI-Desktop/blob/main/docs/使用说明.md)**

## 下载安装

1. 在 Releases 下载 `ATRI-Desktop-v版本号-windows-x64.zip`。
2. 完整解压，双击 `ATRI/ATRI.exe` 或 `Start-ATRI.cmd`。
3. 拖动人物移动；右键打开聊天、衣橱、表情和设置。
4. 需要 AI 聊天时，在“聊天与联动设置”填写自己的 API 地址、模型和密钥。

支持 Windows 10 / 11 x64；已包含 Electron 和模型资源，不需要另装 Node、Python、DSH 或 QQ 机器人。

外观、互动、表情与换装可离线使用。文字聊天支持 OpenAI Chat Completions 兼容服务及本机 Ollama。聊天使用自己的 API 配置和额度，程序不提供公共 API Key。

专属音色与 QQ 联动需要自行部署兼容后端，本包不包含 QQ 登录态、私人机器人、聊天记忆或语音训练权重。详细范围见使用说明。

## 升级与回退

每个版本保存在独立 Release 中。先退出旧版，再将新版解压到新文件夹启动。个人设置和独立聊天记录保存在 `%LOCALAPPDATA%\ATRI Desktop`，升级后继续使用。需要回退时启动旧版即可；涉及数据格式变化的版本以更新说明为准。

用 PowerShell 的 `Get-FileHash -Algorithm SHA256` 对比每个版本附带的 `SHA256SUMS.txt`，确认下载文件完整。

## 后续版本

普通用户只需要下载桌宠 ZIP。`ATRI-Publisher-Kit-v版本号.zip` 是维护者使用的构建工具、冻结源码和资源，不需要普通使用者下载。该工具保存各版 ZIP、哈希、版本目录，拒绝覆盖旧版本。

从自己的开发目录制作新版，运行发行工具中的 `tools/New-Release.ps1`；检查通过后用 `tools/Publish-GitHub.ps1` 上传到同一仓库的 Releases。见 [发布维护说明](发布维护说明.md)。

## 素材与反馈

非官方同人项目，角色形象及模型等素材权利归原权利人。模型作者为远梦清思，当前按非商业同人分享整理；第三方声明和许可证随包保留，不将角色和模型统一授权为 MIT。商业使用请另行确认授权。

问题反馈请附版本、Windows 版本、复现步骤和错误提示。不要上传 API Key、`connection.json`、`host.json` 或私人聊天记录。
