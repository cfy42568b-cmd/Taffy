# 山间牧歌 Alpine Meadow

Three.js 0.170.0 山地牧场微缩场景。原生 ES Modules，无需构建，依赖已放在 dist/vendor 中。

## 本地运行

在项目目录执行 `python3 -m http.server 8000 --directory dist`，浏览器打开 `http://localhost:8000`。请通过 HTTP 运行，避免直接打开 HTML 时的浏览器模块限制。

## 交互

- 拖动旋转、滚轮缩放、右键平移；触屏单指旋转、双指缩放。
- 午后、日落、星夜切换。
- 自动环绕、动画暂停、重置视角、保存 PNG。
- 点击居民或动物打招呼。

## 渲染

支持 WebGL 2 的浏览器使用 MeshToonMaterial、四阶光照渐变、几何轮廓与实时阴影。无法创建 WebGL 上下文时，自动使用 Three.js 官方 SVGRenderer 作软件兼容渲染；兼容模式会降低帧率并省略阴影。

场景、地形、建筑、动物与居民均由代码建模。字体可选在线加载，加载失败时采用系统字体。

Three.js 采用 MIT 许可证，详见 dist/vendor/LICENSE.txt。
