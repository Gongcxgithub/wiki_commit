# 开源项目 CDN 服务

## 简介

镜像优秀开源项目的静态资源以提供高速、可用的 CDN 任播服务

### 特点

---

- 使用腾讯云 CDN 加速
- 提供 7h\*24d 全天候 24 小时不间断服务，如遇服务更新维护会提前 7H 说明
- 中国境内全地可用，延时低于 20ms，且可用性 90 % +（[可用性记录](https://status.gcxstudio.cn)）

---

!> 如果您想使用本服务，请详细阅读文档以便于您更好的进行开发

## 已支持项目

!> 为节省流量及性能开销，除必须标明版本号的项目，均只镜像最新版本以及主流版本

| 项目名                                                    | 项目地址                                             | 版本    | 简介                                                                 |
| --------------------------------------------------------- | ---------------------------------------------------- | ------- | -------------------------------------------------------------------- |
| [Material Design User Interface](https://www.mdui.org/)   | [https://www.mdui.org](\https://www.mdui.org/)       | v1.0.2  | MDUI 漂亮、轻量且好用，它能让你更轻松地开发 Material Design 网页应用 |
| [Bootstrap v5](https://getbootstrap.com)                  | [https://getbootstrap.com](https://getbootstrap.com) | v5.1.3  | Build fast, responsive sites with Bootstrap                          |
| [Argon Theme](https://github.com/solstice23/argon-theme/) | https://github.com/solstice23/argon-theme/           | v1.3.5  | Argon - 一个轻盈、简洁、美观的 WordPress 主题                        |
| [jQuery](https://jquery.com)                              | [https://jquery.com](https://jquery.com)             | v3.6.0  | Fast, small, and feature-rich JavaScript library.                    |
| [Docsify ](https://docsify.js.org)                        | [https://docsify.js.org](https://docsify.js.org)     | v4.12.2 | A magical documentation generator.                                   |
| [Font Awesome Free](https://fontawesome.com)              | [https://fontawesome.com](https://fontawesome.com)   | v6.1.1  | Take the hassle out of icons in your website.                        |

## 调用

按照以下表进行静态资源调用

| 项目名                         | 地址                                                                                                   | 资源路径          | 镜像内容      |
| ------------------------------ | ------------------------------------------------------------------------------------------------------ | ----------------- | ------------- |
| Material Design User Interface | [https://v2.gcxstudio.cn/global-cdn/mdui/](https://v2.gcxstudio.cn/global-cdn/mdui/)                   | Github 发行版路径 | Github 发行版 |
| Bootstrap v5                   | [https://v2.gcxstudio.cn/global-cdn/bootstrap/](https://v2.gcxstudio.cn/global-cdn/bootstrap/)         | 官方资源包路径    | 官方资源包    |
| Argon Theme                    | [https://v2.gcxstudio.cn/global-cdn/argon/v%theme_version%](https://v2.gcxstudio.cn/global-cdn/argon/) | Github 发行版路径 | Github 发行版 |
| jQuery                         | [https://v2.gcxstudio.cn/global-cdn/jquery/version](https://v2.gcxstudio.cn/global-cdn/jquery/)        | 官方资源包路径    | 官方资源包    |
| Docsify & 官方插件             | [https://v2.gcxstudio.cn/global-cdn/docsify ](https://v2.gcxstudio.cn/global-cdn/docsify)              | 官方资源包路径    | Github 发行版 |
| Font Awesome Free              | [https://v2.gcxstudio.cn/global-cdn/font-awesome](https://v2.gcxstudio.cn/font-awesome)                | 官方资源包路径    | 官方资源包    |

路径展示：

```
global-cdn/
├── argon/
│   ├── 目录过于复杂不展示
├── bootstrap/
│   ├── css/
│   ├── js/
├── docsify/
│   ├── lib/
│   ├── pagination/
│   ├── themes/
├── font-awesome/
│   ├── css/
│   ├── js/
│   ├── less/
│   ├── metadata/
│   ├── scss/
│   ├── sprites/
│   ├── svgs/
│   ├── webfonts/
├── jquery/
│   ├── 3.6.0/
├── mdui/
│   ├── css/
│   ├── fonts/
│   ├── icons/
│   ├── js/
├── odometer/
│   ├── odometer.min.js
│   ├── odometer-theme-minimal.css
├── particles/
│   ├── particles.js
│   ├── particles.min.js
├── player/
│   ├── video-js/
│   ├── hls.js/
│   ├── flv.js/
│   ├── dplayer/
│   ├── dashjs/
│   ├── aplayer/
└── v2.gcxstudio.cn
```

## 举例

使用 HTML 调用 MDUI 前端库：

```html
<!-- 调用 MDUI 的 JavaScirpt 资源 -->
<scirpt
  type="text/javascript"
  src="//v2.gcxstudio.cn/global-cdn/mdui/js/mdui.min.js"
  crossorigin="anonymous"
></scirpt>
<!-- 调用 MDUI 的 SCSS 文件 -->
<link
  type="text/css"
  rel="stylesheet"
  href="//v2.gcxstudio.cn/global-cdn/mdui/css/mdui.min.css"
  crossorigin="anonymous"
/>
```

!> 其他前端库调用方法暂不举例

## 其他

本内容仅发布于 [Gong_cx's Wiki](https://docs.gcxstudio.cn)，禁止盗用内容或转载。

!> 服务器为腾讯云上海，配置有限未启用均衡负载，请勿频繁调用本 API 或进行诸如 CC 攻击等此类无耻的行为

## 技术栈

> 本文档使用 [docsify](https://docsify.js.org/) 构建。
