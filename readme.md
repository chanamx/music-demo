- 一个现代化音乐播放器 Demo，包含普通模式与极客模式，核心逻辑在 main.ts
- 普通模式提供大按钮播放控制、场景化一键切换、搜索筛选、收藏、待播队列、实时可视化与音效预设
- 极客模式提供播放倍率、A/B 循环、实时音频诊断、原始状态面板、音源链接复制与快捷键操作
- Demo 采用浏览器内离线合成音轨，不依赖外部流媒体接口，开箱即可演示完整体验
亮点

- 曲库与场景系统定义在 trackBlueprints / scenePresets ，适合继续扩展成真实产品
- 播放器主界面、控制台、队列与普通/极客双模式渲染在 renderPlayerPanel 与 renderGeekPanel
- 离线音轨合成与 Web Audio 处理在 synthesizeTrack 和 ensureAudioGraph
- 场景切换、交互绑定和快捷键逻辑在 bindEvents 与 applyScene
- 现代化视觉样式、主题切换、响应式布局在 style.css
界面设计

- 顶部信息条、玻璃拟态面板、动态背景与深浅主题切换样式见 style.css
- 主播放器、场景卡片、曲库卡片、极客状态面板与代码视图样式见 style.css
- 页面标题与语言已更新为中文，在 index.html