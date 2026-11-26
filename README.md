# HAULMP 聊天翻译

欧卡2 / ATS 的 HaulMP 联机公屏实时翻译工具。Windows 10/11，单文件，下载即用，无需安装。

## 下载

- 官网：https://haulmp-chat-translator.pages.dev
- 直连下载（最新版 v0.8.66，318 MB）：https://haulmp-chat-translator.pages.dev/download/latest.exe
- SHA256：`690000F1495F333AC4FFF88C3DB7DFBB08F4871EC0D97D60835E5DF4BEDB8A60`
- 使用教程：https://haulmp-chat-translator.pages.dev/tutorial.html

## v0.8.66 更新内容

在线翻译通道超时不再逐条硬等：拉丁文本改走并发接口、其它语种直接本地离线，单条翻译从 10~23 秒降到 20~130 毫秒，公屏新消息基本即时出译文。

## 快速上手

1. 双击 `HAULMP聊天翻译.exe` 启动，首次运行会自动拉起语音与离线翻译资源。
2. 进游戏（HaulMP 联机），公屏消息自动抓取并翻成中文，浮窗可拖动、贴底、隐藏。
3. 热键：`C` 显示 / 隐藏浮窗，`R` 回复，`G` 取词，`Ctrl+Alt+B` 语音输入，`T` 透明、`P` 不透明度。
4. 旧版本启动会弹窗问「现在更新吗」，点「立即更新」自动换成新版。

## 说明

- 翻译优先走在线通道（有道 / 腾讯），不通时自动降级到本地离线模型；土耳其语等非拉丁语种直接走本地模型，质量以离线水平为准。
- 语音识别用 whisper medium 量化模型，内置在安装目录 `voice\` 下。
