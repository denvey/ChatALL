<div align="center">
   <img src="src/assets/logo-cover.png" width=256></img>
   <p><strong>同时与所有 AI 机器人聊天，找到最佳答案</strong></p>

[Deutsch](README_DE-DE.md) | [English](README.md) | [Español](README_ES-ES.md) | [Français](README_FR-FR.md) | [Italian](README_IT-IT.md) | [日本語](README_JA-JP.md) | [한국어](README_KO-KR.md) | [Русский](README_RU-RU.md) | [Tiếng Việt](README_VI-VN.md) | 简体中文

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/sunner/ChatALL)

</div>

## 说明
本项目fork自chatall，主要修改了样式和优化了一些用户体验。
样式修改：
- 调整了icon大小
- navbar和底部修改为毛玻璃效果

用户体验:
- 修改了多对话的显示效果，修改为横向滚动查看多个AI的对话内容，支持tab快速切换(还微完成)
- 修复流式回答有点卡(修复中)

## 屏幕截图

![Screenshot](screenshots/screenshot-1.png?raw=true)

## 功能

基于大型语言模型（LLMs）的 AI 机器人非常神奇。然而，它们的行为可能是随机的，不同的机器人在不同的任务上表现也有差异。如果你想获得最佳体验，不要一个一个尝试。ChatALL（中文名：齐叨）可以把一条指令同时发给多个 AI，帮助您发现最好的回答。你需要做的只是[下载、安装](https://github.com/sunner/ChatALL/releases)和提问。

### 这是你吗？

ChatALL 的典型用户是：

- 🤠**大模型重度玩家**，希望从大模型找到最好的答案，或者最好的创作
- 🤓**大模型研究者**，直观比较各种大模型在不同领域的优劣
- 😎**大模型应用开发者**，快速调试 prompt，寻找表现最佳的基础模型

### 支持的 AI

| AI 机器人                                                                      | 网页访问 | API      | 说明                                     |
| ------------------------------------------------------------------------------ | -------- | -------- | ---------------------------------------- |
| [ChatGPT](https://chat.openai.com)                                             | 支持     | 支持     | 包含 Web Browsing、Azure OpenAI service  |
| [Copilot](https://copilot.microsoft.com/)                                      | 支持     | 无 API   | 不需要帐号                               |
| [文心一言](https://yiyan.baidu.com/)                                           | 否       | 支持     |                                          |
| [Gemini](https://gemini.google.com/)                                           | 支持     | 即将推出 |                                          |
| [Poe](https://poe.com/)                                                        | 支持     | 即将推出 |                                          |
| [MOSS](https://moss.fastnlp.top/)                                              | 支持     | 无 API   |                                          |
| [通义千问](http://tongyi.aliyun.com/)                                          | 支持     | 即将推出 |                                          |
| [得到学习助手](https://ai.dedao.cn/)                                           | 即将推出 | 无 API   |                                          |
| [讯飞星火](http://xinghuo.xfyun.cn/)                                           | 支持     | 即将推出 |                                          |
| [Vicuna 13B 和 33B](https://lmsys.org/blog/2023-03-30-vicuna/)                 | 支持     | 无 API   | 不需要帐号                               |
| [ChatGLM2 6B 和 130B](https://chatglm.cn/blog)                                 | 支持     | 无 API   | 不需要帐号                               |
| [Claude 2 和 Instant](https://www.anthropic.com/index/claude-2)                | 支持     | 无 API   | 不需要帐号                               |
| [Gradio](httpps://gradio.app/)                                                 | 支持     | 无 API   | 用于 Hugging Face space 或自己部署的模型 |
| [HuggingChat](https://huggingface.co/chat/)                                    | 支持     | 无 API   |
| [天工](https://neice.tiangong.cn/)                                             | 支持     | 即将推出 |                                          |
| [You](https://you.com/)                                                        | 支持     | 无 API   |                                          |
| [Pi](https://pi.ai)                                                            | 支持     | 无 API   |                                          |
| [360 智脑](https://ai.360.cn/)                                                 | 支持     | 无       |                                          |
| [YouChat](https://you.com/)                                                    | 支持     | 无       |                                          |
| [Open Assistant](https://open-assistant.io/)                                   | 支持     | 无       |                                          |
| [Character.AI](https://character.ai/)                                          | 支持     | 无       |                                          |
| [Llama 2 13B 和 70B](https://ai.meta.com/llama/)                               | 支持     | 无 API   |                                          |
| [Code Llama](https://ai.meta.com/blog/code-llama-large-language-model-coding/) | 支持     | 无 API   |                                          |
| [WizardLM 70B](https://github.com/nlpxucan/WizardLM)                           | 支持     | 无 API   |                                          |
| [Falcon 180B](https://huggingface.co/tiiuae/falcon-180B-chat)                  | 支持     | 无 API   |                                          |
| [Phind](https://www.phind.com/)                                                | 支持     | 无 API   |                                          |

还会有更多。[到这里](https://github.com/sunner/ChatALL/labels/more%20LLMs)为你喜欢的 AI 投票吧。

### 其他功能

- 快问模式：不需要等待前面的请求完成，就可以发下一条指令
- 对话历史保存在本地，保护你的隐私
- 高亮喜欢的答案，删除不需要的答案
- 随时启用/禁用任何机器人
- 在一列、两列或三列视图之间切换
- 自动更新到最新版
- 夜间模式（由 @tanchekwei 贡献）
- 快捷键。按 <kbd>Ctrl</kbd> + <kbd>/</kbd> 可以看到所有快捷键（由 @tanchekwei 贡献）
- 多对话窗口（由 @tanchekwei 贡献）
- 支持设置代理（由 @msaong 贡献）
- 提示词管理（由 @tanchekwei 贡献）
- 支持多语言（中文、英语、德语、法语、俄语、越南语、韩语、日语、西班牙语、意大利语）
- 支持 Windows，macOS 和 Linux

计划中：

欢迎参与这些功能的开发。

- [ ] 把前端部署到 GitHub Pages

## 隐私

所有的聊天记录、设置和登录数据都保存在您的计算机本地。

ChatALL 收集匿名的使用数据，以帮助我们改进产品。包括：

- 向哪些 AI 机器人发送了提示词，以及提示词的长度。不包括提示词内容
- AI 回复的长度，以及哪些回复被删除/高亮显示。不包括回复内容

## 预先需要

ChatALL 是一个客户端，而不是代理。因此，您必须：

1. 拥有可以访问这些 AI 的帐号，或 API token。
2. 与 AI 网站有可靠的网络连接。

## 下载 / 安装

从 https://github.com/sunner/ChatALL/releases 下载

### Windows 系统

直接下载 \*-win.exe 安装文件并运行之。

### macOS 系统

对于苹果硅芯片 Mac（M1，M2 CPU），请下载 \*-mac-arm64.dmg 文件。

对于其他 Mac，下载 \*-mac-x64.dmg 文件。

如果你在使用 [Homebrew](https://brew.sh/)，可以使用以下命令安装：

```bash
brew install --cask chatall
```

### Linux 系统

下载 .AppImage 文件，将其设置为可执行，然后双击就可运行。

## 问题解决

使用中如果遇到问题，可以尝试如下方法解决：

1. **刷新** - 按下 <kbd>Ctrl</kbd> + <kbd>R</kbd> 或 <kbd>⌘</kbd> + <kbd>R</kbd>。
2. **重启** - 退出 ChatALL，再重新运行。
3. **重新登录** - 点击右上角的设置按钮，在弹出的窗口中点击对应的登入/登出链接，重新登录网站。
4. **创建新对话** - 创建一个新对话，再发送提示词。

如果以上方法都不行，那么可以尝试**重置 ChatALL**。注意，这将丢失你所有的设置和消息历史。

删除下面的目录可以重置 ChatALL：

- Windows: `C:\Users\<user>\AppData\Roaming\chatall\`
- Linux: `/home/<user>/.config/chatall/`
- macOS: `/Users/<user>/Library/Application Support/chatall/`

如果问题依旧，请[提交一个 issue](https://github.com/sunner/ChatALL/issues)。

## 给开发者

### 贡献新的 AI 机器人

[这份文档](https://github.com/sunner/ChatALL/wiki/%E5%A6%82%E4%BD%95%E6%B7%BB%E5%8A%A0%E4%B8%80%E4%B8%AA%E6%96%B0%E7%9A%84-AI-%E5%AF%B9%E8%AF%9D%E6%9C%BA%E5%99%A8%E4%BA%BA)能提供一些帮助。

### Run

```bash
npm install
npm run electron:serve
```

### Build

为您当前的平台构建：

```bash
npm run electron:build
```

为所有平台构建：

```bash
npm run electron:build -- -wml --x64 --arm64
```

## 致谢

### 贡献者

<a href="https://github.com/sunner/ChatALL/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=sunner/ChatALL" />
</a>

### 其它

- GPT-4 贡献了大部分代码
- ChatGPT，Copilot 和 Google 提供了许多解决方案（排名分先后）
- 受 [ChatHub](https://github.com/chathub-dev/chathub) 启发。致敬！

## 赞助

本项目的支持经费来自于：

1. [AI 大模型全栈工程师培养计划 - AGIClass.ai](https://agiclass.ai)
2. [孙志岗讲解 AI 为什么](https://note.mowen.cn/note-intro/?noteUuid=vKwymX8n5BEpqD5nCZPRo)

欢迎传播、购买以上课程和专栏来支持本项目，谢谢。
