# ST 预设裁剪工具

轻量级 SillyTavern 预设 JSON 编辑器，纯前端单文件应用，无需安装任何依赖。

## 功能

- **文件导入** — 拖拽或点击选择 JSON 预设文件
- **条目管理** — 查看所有 prompt 的名称、角色类型、depth、order
- **开关切换** — 每个条目可独立切换 enabled 状态
- **内容编辑** — 展开卡片编辑 content 文本
- **撤销/重做** — 支持 Ctrl+Z / Ctrl+Y，最多 50 步历史
- **重置** — 一键恢复预设原始状态，可随时撤回
- **搜索过滤** — 按名称实时搜索条目
- **全选** — 一键开启/关闭所有条目
- **导出** — 仅保留 enabled 条目，生成裁剪后的 JSON 文件
- **日/夜间模式** — 跟随系统设置，也可手动切换

## 使用方法

双击 `index.html` 即可在浏览器中直接使用，零配置零依赖。

## 技术栈

- HTML5 + CSS3 + JavaScript（单文件）
- 原生 File API / Blob API
- CSS Custom Properties 实现主题系统
- Google Fonts（DM Sans + Instrument Sans + JetBrains Mono）

## 设计

采用精致工具感设计语言，参考 Linear / Raycast 风格：
- 三层 CSS Token 架构（Primitives → Semantic → Component）
- WCAG AA 无障碍对比度标准
- `prefers-reduced-motion` 无障碍动画支持
- 玻璃拟态 + 噪点纹理背景

## 许可

MIT
