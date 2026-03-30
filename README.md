# zoogent

## 计划功能
- [x] 设置角色可在屏幕上二维移动
- [x] 设置角色可拖拽
- [x] 显示的对话窗口根据角色的位置动态调整，确保对话窗口不会被角色遮挡或出现在屏幕边缘
- [ ] 新角色
- [ ] 设计菜单图标
- [ ] 设计app icon
- [ ] 角色
  - [ ] 增加更多的角色，比如猫、狗、兔子等，增加趣味性。
  - [ ] 角色位置可固定
  - [ ] 增加角色的表情和动作，比如跳出屏幕，移动到屏幕边缘等，增加互动性。
  - [ ] 增加角色的声音，比如叫声、笑声等，增加趣味性。
  - [ ] 增加自定义角色的功能，用户可以上传自己的角色图片和声音，增加个性化。
  - [ ] 角色记忆功能 
  - [ ] 保存对话记录 压缩对话
  - [ ] 自定义角色性格
  - [ ] 角色会根据对话内容做出不同的表情和动作
  - [ ] 对话框样式调整
- [ ] 自定义 api 接口
  - [ ] 不同的agent设置不同的api
- [ ] 自定义 skill
- [ ] Game mode：角色可以在屏幕上进行一些简单的游戏，比如捉迷藏、跳绳等，增加娱乐性。

![zoogent](hero-thumbnail.jpg)

Tiny AI companions that live on your macOS dock.

**Bruce** and **Jazz** walk back and forth above your dock. Click one to open an AI terminal. They walk, they think, they vibe.

Supports **Claude Code**, **OpenAI Codex**, and **GitHub Copilot** CLIs — switch between them from the menubar.

## open source attribution

This project is based on the open-source project [lil-agents](https://github.com/ryanstephen/lil-agents).
zoogent extends and customizes that work for this repository.

## maintainer

- Author: Guo Yiheng
- GitHub: [@guoyiheng](https://github.com/guoyiheng)

## features

- Animated characters rendered from transparent HEVC video
- Click a character to chat with AI in a themed popover terminal
- Switch between Claude, Codex, and Copilot from the menubar
- Four visual themes: Peach, Midnight, Cloud, Moss
- Thinking bubbles with playful phrases while your agent works
- Sound effects on completion
- First-run onboarding with a friendly welcome
- Auto-updates via Sparkle

## requirements

- macOS Sonoma (14.0+)
- At least one supported CLI installed:
  - [Claude Code](https://claude.ai/download) — `curl -fsSL https://claude.ai/install.sh | sh`
  - [OpenAI Codex](https://github.com/openai/codex) — `npm install -g @openai/codex`
  - [GitHub Copilot](https://github.com/github/copilot-cli) — `brew install copilot-cli`

## building

Open `zoogent.xcodeproj` in Xcode and hit run.

## privacy

zoogent runs entirely on your Mac and sends no personal data anywhere.

- **Your data stays local.** The app plays bundled animations and calculates your dock size to position the characters. No project data, file paths, or personal information is collected or transmitted.
- **AI providers.** Conversations are handled entirely by the CLI process you choose (Claude, Codex, or Copilot) running locally. zoogent does not intercept, store, or transmit your chat content. Any data sent to the provider is governed by their respective terms and privacy policies.
- **No accounts.** No login, no user database, no analytics in the app.
- **Updates.** zoogent uses Sparkle to check for updates, which sends your app version and macOS version. Nothing else.

## license

MIT License. See [LICENSE](LICENSE) for details.
