# PulseLab 音乐播放器 Demo

一个现代化的浏览器音乐播放器 Demo，采用 TypeScript + Vite 构建，支持普通模式与极客模式双界面。

## 特性

### 普通模式
- 🎵 大按钮播放控制
- 🎭 场景化一键切换
- 🔍 搜索筛选功能
- ⭐ 收藏管理
- 📋 待播队列
- 📊 实时音频可视化
- 🎛️ 音效预设

### 极客模式
- ⚡ 播放倍率调节
- 🔁 A/B 循环
- 🔬 实时音频诊断
- 📈 原始状态面板
- 🔗 音源链接复制
- ⌨️ 快捷键操作

## 技术亮点

- **曲库与场景系统**：定义在 `trackBlueprints` / `scenePresets`，适合扩展成真实产品
- **双模式渲染**：主播放器、控制台、队列与普通/极客模式分别在 `renderPlayerPanel` 与 `renderGeekPanel`
- **音频处理**：离线音轨合成与 Web Audio 处理在 `synthesizeTrack` 和 `ensureAudioGraph`
- **交互逻辑**：场景切换、事件绑定和快捷键逻辑在 `bindEvents` 与 `applyScene`
- **视觉设计**：现代化样式、主题切换、响应式布局在 `style.css`

## 界面设计

- 顶部信息条、玻璃拟态面板、动态背景与深浅主题切换
- 主播放器、场景卡片、曲库卡片、极客状态面板与代码视图
- 中文界面，已本地化

## 快速开始

```bash
安装依赖
npm install

开发模式
npm run dev

构建生产版本
npm run build

预览构建结果
npm run preview
```

## 技术栈

- **TypeScript** - 类型安全的 JavaScript
- **Vite** - 下一代前端构建工具
- **Web Audio API** - 浏览器原生音频处理

## 注意事项

Demo 采用浏览器内离线合成音轨，不依赖外部流媒体接口，开箱即可演示完整体验。

## License

MIT
