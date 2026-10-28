# Personal AI System｜正式网站部署

正式域名：<https://ai.zxyzx.me/>。此仓库仅存放 GitHub Pages 自动部署工作流，不维护另一个网站源码。

工作流从唯一源码仓库 `zxyzx0430/personal-ai-web` 的 `main` 分支检出 React + TypeScript + Vite 代码，运行 `npm ci`、类型检查、Lint、相对路径构建与静态文件完整性检查，然后把 **完整的 `dist/`** 发布到 GitHub Pages（包括 HTML、CSS、JS、3 份 PDF 与学习演示视频）。

当源码升级时，可以到 Actions → Publish Personal AI website → Run workflow 手动刷新正式站；此外每天自动重新发布。原正式站发布工作流只复制 HTML 文件的做法已经弃用，避免 React 的 CSS/JS/视频缺失而造成白屏。

上线前的主分支备份保存在 `backup/pre-react-motion-20261028`。维护与功能修改应在唯一源码仓库进行。
