---
title: "山间牧歌：用 Three.js 搭建一个山地牧场小镇"
date: 2026-11-15
tags: [Three.js, 程序设计, 三渲二]
---

# 山间牧歌

雪峰之下，溪流穿过木屋小镇，流向牛羊成群的牧场。八位像素居民沿着镇前道路和草坡散步。

- [阅读全文与体验](https://taffy.xin/2026/11/15/alpine-meadow/)
- [独立打开场景](https://taffy.xin/programs/alpine-meadow/)
- [完整源码](../alpine-meadow/)

## 场景内容

六座木屋、雪山、溪流、木桥、松树与牧场；八头奶牛、十只小羊与八位居民。

## 操作

拖动旋转、滚轮缩放、右键平移；触屏单指旋转、双指缩放。点击居民或动物打招呼。工具栏可切换午后、日落与星夜，开启自动环绕、暂停动画、重置视角或保存 PNG 风景。

## 技术

Three.js 0.170.0，原生 ES Modules，程序化几何建模、卡通材质、几何轮廓与实时阴影。依赖随项目提供。无法创建 WebGL 上下文时自动使用 Three.js 官方 SVGRenderer 兼容渲染，省略实时阴影并降低动画帧率。

## 本地运行

进入 alpine-meadow 目录，执行：

```bash
python -m http.server 8000 --directory dist
```

在浏览器中访问 http://localhost:8000。
