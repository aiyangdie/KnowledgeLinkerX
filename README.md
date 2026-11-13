<p align="center"><img src="assets/covers/08-KnowledgeLinkerX.jpg" alt="小程序导航 项目封面" width="100%"></p>

<h1 align="center">KnowledgeLinkerX · 小程序导航页</h1>

<p align="center">把多个小程序与公众号的图标、二维码收在一页，扫码即达</p>

<p align="center">
  <a href="http://knowledge.aikex.ink/">在线访问</a> ·
  <a href="https://github.com/aiyangdie/KnowledgeLinkerX">源码仓库</a>
</p>

## 简介

一个纯静态的导航页，用来集中展示自己或团队的小程序与公众号入口。卡片式布局按分类排布，每张卡包含图标、名称和二维码，手机上扫码直接进小程序，不需要额外开发。

## 功能

- **分类展示**：微信小程序、QQ 小程序、公众号三个分区，用分隔线区分
- **卡片布局**：图标 + 名称 + 二维码，一卡一入口
- **悬停动效**：鼠标移上去卡片上浮、阴影加深
- **响应式**：Flexbox 弹性布局，手机与桌面都能看
- **零依赖**：一个 HTML + 一份 CSS + 图片目录，丢到任何静态托管即可

## 技术栈

HTML5 · CSS3（Flexbox / 渐变 / 过渡 / 圆角阴影）· 本地图片资源

## 快速开始

```bash
git clone https://github.com/aiyangdie/KnowledgeLinkerX.git
```

直接用浏览器打开 `index.html`。

## 添加自己的入口

1. 把图标与二维码放进 `images/`，建议成对命名（如 `xxx_icon.png`、`xxx_qrcode.jpg`）
2. 在 `index.html` 里加一块卡片：

```html
<div class="app-item">
  <img src="images/your_icon.png" alt="小程序名称" class="app-icon">
  <h2>小程序名称</h2>
  <img src="images/your_qrcode.jpg" alt="小程序名称二维码" class="app-qrcode">
</div>
```

3. 需要分组时插一行 `<hr class="separator">`

## 项目结构

```
index.html        主页面
styles.css        样式
images/           各小程序的图标与二维码
CNAME             自定义域名配置
```

## 许可证

仓库未附 LICENSE 文件，使用与分发请先联系作者确认。
