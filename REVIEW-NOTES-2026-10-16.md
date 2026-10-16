# 核对反馈（2026-10-16）· 七七

对照 10-15 发布记录，今天上午预览站的 5 个移动端修复回流情况核对如下：

- ✅ 卡片对齐（fa321a98）：源头分支有对应提交。
- ⚪ 样式导入路径（f50392ab）、缓存刷新（9663f76c）：Pages 部署专属，无需回流。
- ✅ 工作台导航压缩（14045a52）：净效果源头分支已具备（逐行 diff 仅差 3 行预览品牌样式）。
- ❌ **移动端排版与流程（4b28f7a5）未回流**：`.headline-line` / `.flow-arrow` / `.story-stage` 弹性布局 / clamp 字号 / `.method-strip` 不换行——预览站已生效，但源头分支的 landing.css、landing.html 仍是旧版绝对定位写法。建议回流。

⚠️ 线上 `preview-manifest.json` 的 `sourceCommit`（a007143a）在源头分支历史中无法解析（无此提交），疑似记录了构建快照或过期 SHA。建议修正 manifest 生成逻辑，保证 `sourceCommit` / `reviewedMain` 可解析，发布记录才可追溯。

（详细核对过程见团队私有渠道。）
