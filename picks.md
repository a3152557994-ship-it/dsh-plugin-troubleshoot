# 48 个近期维护中的 DSH 插件（2026-11 快照）

> 筛选条件：近 30 天有更新 + 有中文描述 + 声明了 DSH 版本要求；按 star 与活跃度排序。
> 安装：`dsh plugin --profile <你的profile> add <包名>`；装之前对照最后一列的版本要求。

| # | 插件 | 用途 | 分类 | 更新时间 | star | 要求 DSH 版本 |
|---|---|---|---|---|---|---|
| 1 | ``dsh-vision-router`` | 为纯文本 Agent 提供视觉能力：内置免 Key 视觉链 + 像素级视觉工具（ | 视觉 | 11-06 | 1237 | >=0.1.5-rc.1 <0.2.0- |
| 2 | ``dsh-mnemon`` | 由 Mnemon 驱动的 DeepSeek Harness（DSH）跨 Agen | 记忆 | 11-06 | 915 | >=0.2.0-rc.2 <0.2.1- |
| 3 | ``dsh-free-search`` | DSH 免费搜索插件：7 个引擎（DuckDuckGo/Bing/SearXNG | 浏览器 | 11-07 | 966 | 未声明 |
| 4 | ``@anionex/dsh-vision-toolkit`` | 让纯文本模型处理视觉任务：粘贴图片后自动切换到 Vision Toolkit 变 | 视觉 | 11-07 | 930 | 未声明 |
| 5 | ``dsh-openwrite`` | 面向 DSH 的小说创作工作台，提供创作预设、大纲与人物管理、正文批注、审稿流程 | 工作流 | 11-07 | 930 | 未声明 |
| 6 | ``dsh-video-storyboard`` | 把视频（本地文件，或 B 站 / yt-dlp 链接）压成一张可寻址的宫格图：每 | 视觉 | 11-06 | 458 | 未声明 |
| 7 | ``dsh-see-now`` | 让只有文字的智能体「看」实时屏幕或摄像头：每帧按画面变化量打分，只把真正变了的帧 | 视觉 | 11-06 | 441 | 未声明 |
| 8 | ``dsh-opencode-go`` | OpenCode Go 模型提供方，支持网关实时模型发现、models.dev  | 模型接入 | 11-07 | 268 | >=0.2.1-rc.5 |
| 9 | ``dsh-rewind-plugin`` | 对话回退：一键回到任意更早的用户消息，同窗口内完成，不新建分支、不残留副本；目标 | 会话 | 11-07 | 244 | >=0.2.2-rc.1 <0.3.0- |
| 10 | ``@nagi-ovo/dsh-visualize`` | 对话内生成式 UI：模型把交互式 HTML 卡片直接画进会话流，带流式预览与沙箱 | 界面 | 11-07 | 336 | 未声明 |
| 11 | ``dsh-config-manager`` | 一键备份、导出、导入与迁移整套 DSH 配置：设置、插件、MCP、技能与工作区。 | 工具 | 11-07 | 309 | 未声明 |
| 12 | ``@zaofan/dsh-qqbot`` | 接入 QQ 官方机器人的 DeepSeek Harness 通道(tencent | 通知 | 11-07 | 230 | 未声明 |
| 13 | ``memory-eternal`` | 别的记忆插件让 AI 记住更多，我们让 AI 只记住对的：Agent 只能提案， | 记忆 | 11-07 | 147 | >=0.1.5-alpha.2 <0.3 |
| 14 | ``@michengai/dsh-im-connect`` | 把微信、企业微信、钉钉、飞书、Lark、QQ、Telegram 接到本机 Dee | 通知 | 11-06 | 126 | >=0.2.0-rc.1 <0.3.0- |
| 15 | ``stratagate-dsh`` | 近期对话保持清晰，久远记忆逐渐化为摘要，而不是消失。StrataGate 为 D | 记忆 | 11-07 | 116 | 0.1.2-rc.1 // >=0.1. |
| 16 | ``dsh-agy-link`` | 将 Google Antigravity (agy CLI) 接入 DSH：无  | 模型接入 | 11-07 | 155 | 未声明 |
| 17 | ``@anionex/dsh-turn-rewind`` | 对话回退：基于持久 Change Ledger 回滚会话与工作区状态。 | 会话 | 11-07 | 145 | 未声明 |
| 18 | ``envoy-dsh`` | 贴一条链接，Agent 直接把内容读给你：小红书笔记、抖音与 B 站视频、微信公 | 浏览器 | 11-07 | 98 | >=0.1.5 |
| 19 | ``@kenz1117/dsh-ui-usage-billing`` | 侧边栏计费仪表盘：从会话日志聚合真实用量（按模型/按日统计调用、Token、缓存 | 用量/计费 | 11-07 | 95 | >=0.1.2-alpha.1 |
| 20 | ``dsh-easyrewrite`` | 在 dsh web 中内联编辑与撤回自己的消息——惰性、无痕，带版本翻页器与会话 | 会话 | 11-07 | 129 | 未声明 |
| 21 | ``dsh-think-translate`` | DSH Web 显示层翻译：思考链、任务、可选回答和审查拒绝理由，支持 9 种语 | 界面 | 11-07 | 75 | >=0.1.0-rc.6 |
| 22 | ``dsh-zotero`` | 面向 Agent 研究工作流的 Zotero 插件：搜索文献、查看元数据与笔记、 | 工具 | 11-06 | 68 | >=0.2.2-rc.1 |
| 23 | ``@anionex/dsh-computer-use`` | macOS 电脑控制：Accessibility 观测、过期状态拒绝、作用域权限 | 工具 | 11-07 | 95 | 未声明 |
| 24 | ``dsh-plugin-guide`` | DSH 插件开发知识库，作为按需加载的 agent 技能随 bundle 安装： | 技能 | 11-07 | 65 | >=0.2.2-0 <0.3.0 |
| 25 | ``dsh-profile-stats`` | DSH 侧栏的个人用量主页，数据全部由本机会话日志经 ctx.sessionQu | 用量/计费 | 11-06 | 56 | >=0.2.1-rc.5 <0.3.0- |
| 26 | ``@hyzyn/dsh-docker`` | DSH Web GUI 的 Docker 容器面板：本机或 SSH 主机上的容器 | 工具 | 11-07 | 64 | 未声明 |
| 27 | ``dsh-game-daily`` | Windows 上的原神 / 崩坏3 / 崩坏：星穹铁道 / 绝区零日常自动化： | 工具 | 11-07 | 43 | >=0.2.0-rc.1 |
| 28 | ``@michengai/dsh-automation`` | 在独立会话里按计划执行编码任务，可在设置页或对话里管理。 | 工作流 | 11-07 | 39 | >=0.2.0-rc.1 <0.3.0- |
| 29 | ``dsh-email`` | 邮件工具插件：含 email_watch 增量新邮件检查、email_mark（ | 通知 | 11-07 | 39 | >=0.2.1-rc.3 |
| 30 | ``dsh-better-workspace`` | DSH 侧边栏「工作区」列表的层级树插件：工作区与会话名称中的 / 即虚拟分组（ | 界面 | 11-07 | 32 | >=0.2.2-rc.1 |
| 31 | ``dsh-workbuddy-bridge`` | 把 WorkBuddy 桌面 App 的模型接进 DSH 模型选择器：国内版与国 | 模型接入 | 11-07 | 30 | ^0.1.7-rc.1 // ^0.2. |
| 32 | ``dsh-cliworker-now`` | 适用于 macOS / Windows 和 DeepSeek Harness 0 | 工作流 | 11-07 | 38 | 未声明 |
| 33 | ``dsh-prime-memory`` | 分层记忆插件，面向 Agent 暴露 10 个工具：高权限写入（memory_a | 记忆 | 11-06 | 25 | >=0.1.1-rc.2 <0.3.0 |
| 34 | ``dsh-session-superagent`` | 会话级 superagent：盯一个 GitHub 仓库，issue/PR 有变 | 会话 | 11-07 | 23 | >=0.2.1-rc.5 <0.2.2- |
| 35 | ``dsh-design-studio`` | 右侧栏的设计工作台。模型做网页、App 界面、桌面软件窗口、微信小程序、海报、幻 | 界面 | 11-07 | 32 | 未声明 |
| 36 | ``dsh-watch-together`` | 和只有文字的智能体一起看视频：需要 ffmpeg 和浏览器扩展上报真实播放位置（ | 语音 | 11-06 | 24 | 未声明 |
| 37 | ``@goodandready/dsh-subscriptions`` | 通过 OAuth 将 ChatGPT Codex、Claude、Grok 与 A | 模型接入 | 11-07 | 23 | 未声明 |
| 38 | ``dsh-zhihu-search`` | 为 DSH 增加三个知乎工具——站内问答与文章检索、知乎全网索引检索（可按域名与 | 工具 | 11-07 | 19 | ^0.1.7-rc.1 // ^0.2. |
| 39 | ``dsh-thinking-levels`` | DSH 逐轮思考级别（reasoning_effort）控制：选择 Auto 即 | 模型接入 | 11-06 | 15 | >=0.1.1-rc.2 <0.3.0 |
| 40 | ``dsh-office-kit`` | 通过 `/documents`、`/pdf`、`/presentations`、 | 文档 | 11-07 | 19 | 未声明 |
| 41 | ``dsh-onebot-qq`` | 给 dsh 加上 QQ 通道（OneBot 11，兼容 NapCat）：反向/正 | 通知 | 11-07 | 12 | >=0.1.5-rc.1 <0.1.6- |
| 42 | ``@crosery/dsh-viewer`` | 面向模型的 display_file 工具，在网页 UI 内联渲染 36 种扩展 | 界面 | 11-06 | 11 | >=0.0.1-rc.0 <0.0.2- |
| 43 | ``dsh-markdown-typora`` | DSH 右侧栏的 Typora 式 Markdown 编辑器：公式与 Merma | 文档 | 11-07 | 11 | >=0.2.0-rc.2 |
| 44 | ``@morehao/dsh-github-trending`` | 按日 / 周 / 月周期定时生成 GitHub 趋势日报，由本地 trendra | 工作流 | 11-07 | 10 | >=0.2.1-rc.3 <0.3.0- |
| 45 | ``dsh-context-compression-improved`` | 机制上与上下文压缩领域最响的两条公开路线同源：代码骨架闸门沿用 Headroom | 会话 | 11-06 | 9 | >=0.1.1-rc.2 <0.3.0 |
| 46 | ``dsh-fast-mode`` | DeepSeek Harness 自己的 fast mode：同一个模型、同样的 | 用量/计费 | 11-07 | 9 | >=0.2.0-rc.1 |
| 47 | ``dsh-plugin-debugging`` | DSH 插件运行时诊断：区分实时生效、重启和热重载。 | 开发 | 11-07 | 9 | ^0.1.7-rc.1 // ^0.2. |
| 48 | ``@goodandready/dsh-cron`` | 为 DeepSeek Harness 提供定时任务、后台自动化与 Agent 执 | 工作流 | 11-07 | 13 | 未声明 |

> 数据来源：awesome-dsh-plugin / dsh-plugin-catalog（2026-11-07 快照）。star 数会随时间变。