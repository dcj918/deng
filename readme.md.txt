
## ✨ 项目概述
本项目是一个响应式天气预报单页应用，采用玻璃拟态UI设计风格，支持**手动输入城市查询天气**与**浏览器自动定位获取天气**两大核心能力，调用和风天气开放API拉取实时天气与三日预报数据，页面加入过渡动画、微动效、加载状态反馈，兼容PC端与移动端，界面精致现代。

## 🚀 功能清单
1. 城市名称检索天气（点击按钮/回车快捷查询）
2. 浏览器Geolocation自动定位，根据经纬度反查城市天气
3. 展示城市名、天气图标、实时温度、天气状况描述
4. 展示未来三日天气预报（日期、天气图标、温度区间）
5. 加载中状态提示、异常捕获与友好弹窗提示
6. 响应式布局，手机端自动适配纵向排版
7. 玻璃拟态磨砂卡片、入场动画、hover微交互、聚焦发光效果

## 🛠️ 核心技术栈
- **HTML5**：语义化结构、viewport移动端适配、Geolocation定位API
- **CSS3**：渐变背景、backdrop-filter玻璃拟态、Flex/Grid弹性布局、animation过渡动画、媒体查询响应式
- **JavaScript(ES6+)**：async/await异步请求、fetch网络请求、事件监听、DOM动态渲染、封装工具函数
- **第三方接口**：和风天气Geo地理编码API、实时天气API、逐日预报API

## 📝 关键技术与代码说明
### 1. UI视觉实现（玻璃拟态+动画）
使用CSS实现磨砂玻璃效果：
```css
.glass-card {
  background: rgba(255,255,255,0.16);
  backdrop-filter: blur(14px);
  border-radius: 22px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.12);
  transition: transform 0.28s ease;
}