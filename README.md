# Referral Incentive Builder · Pipeline Demo

一张可交互的流程节点图，演示「从一份 PRD 到一张可验收的 Lynx 激励页面」的装配式生成流水线原理：

- 两台 390×845 页面直接作为流程节点（Framework 灰坯 / ui-skin 换肤后），共享同一份 assembly plan
- 悬停页面槽位可就地切换组件变体，两台页面实时联动
- 概念图 → 原子 fork 三路并行（clean 背景 / RGBA 主体 / 18 Token）→ join → 机器验收 → 唯一一次构建发布
- 「▶ 运行流水线」播放全链路动画；`#run` 深链接自动播放
- 内置 **3 套真实 run 皮肤**（樱空收集 / 秋暮饼干 / 空飞双六），概念图与三路产物节点全程联动；`?skin=cute|autumn|sugoroku` 深链接直达
- **机型自适应**：顶栏全局切换 320×568 / 390×845（基线钉扎）/ 430×932 / 1024×1366，两台页面同步过渡动画，组件库 clamp/min 自适应表达式按真视口活解析（iframe 隔离，与 Playground 同机制）；`?preset=se|base|max|pad` 深链接直达
- **两阶段双入口**：点 PRD 卡换一份 PRD = 阶段二 AI 重跑全链路生成；点最终页下方皮肤 chips = 阶段一设计师手动 Vibe Coding 换肤（即时、不经 AI）

**在线体验**：开启 GitHub Pages 后访问 `https://<user>.github.io/<repo>/`

纯静态单文件（`index.html`），无任何外部依赖，本地双击亦可打开。
