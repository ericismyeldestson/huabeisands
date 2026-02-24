# 华北沙尘实时监测可视化

本项目是一个基于 HTML5 Canvas 和 Leaflet 的实时监测可视化工具，专门用于显示中国华北地区的沙尘暴（PM10）状况。

## 功能特点

- **动态流动粒子系统**：基于实时风场数据驱动的沙尘流动效果。
- **实时数据接入**：集成 Open-Meteo 空气质量与气象 API，获取最新的 PM10 及风速风向数据。
- **地理插值（IDW）**：使用反距离权重插值算法，将有限的采样点数据平滑扩展至整个华北区域。
- **城市搜索查询**：支持搜索特定城市（如北京、天津等），实时计算该位置的 PM10 浓度、AQI 等级及风力状况，并自动定位。
- **软边缘裁剪**：沙尘粒子严格限制在华北数据覆盖范围内（36-44°N, 110-120°E），并带有自然的边缘淡出效果。
- **精美视觉效果**：采用 Esri 卫星底图，结合 Apple 风格的米色透明 UI 面板，支持 Retina/高分屏。

## 技术栈

- **前端**: HTML5, CSS3, Vanilla JavaScript
- **地图基础**: [Leaflet.js](https://leafletjs.com/)
- **地图瓦片**: Esri World Imagery (卫星图) & Carto Light Labels (标注)
- **数据源**: [Open-Meteo API](https://open-meteo.com/)
- **地理编码**: OpenStreetMap Nominatim

## 本地运行

1. 下载或克隆本项目。
2. 直接在浏览器中打开 `index.html`（建议将 `dust_visualization_fixed.html` 重命名为 `index.html`）。

## 截图预览

*(可以在此处添加截图)*
