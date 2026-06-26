# LEI · Personal Portfolio

> 暗色系响应式个人作品集网站，展示 UI/UX 设计、AIGC 创意、影视与品牌作品。

🌐 **[在线预览 →](https://guyinge.github.io/uiux-portfolio/)**

---

## 项目简介

这是一个纯静态的个人作品集网站，采用暗色系设计语言，融合紫粉渐变光晕、自定义光标交互、滚动揭示动画等视觉元素。网站包含主作品集页面与多个项目详情子页面，完整呈现设计作品的全链路思考与落地。

## ✨ 核心特性

- **暗色系响应式布局** — CSS Grid + `clamp()` + media queries，全设备自适应
- **自定义全局光标** — `cursor:none` + `requestAnimationFrame` 缓动跟随的白色小球
- **紫光球交互** — 不规则形状 `border-radius` 形变 + `radial-gradient` + `blur`，hover 触发紫粉渐变旋转
- **逐行标题 hover** — Hero 标题逐行触发亮紫色 `#c084fc` 高亮
- **滚动揭示动画** — `IntersectionObserver` 实现元素进场过渡
- **纯 CSS 星标** — `clip-path` 绘制五角星，替代 emoji 避免渲染问题
- **多页面导航** — `index.html` → `ziruim.html`（自如链路改版 Case Study）→ `ziruim-app.html`（自如 APP 项目详情）

## 🗂 项目结构

```
.
├── index.html              # 主页：Hero / Works / Experience / Skills
├── ziruim.html             # 自如链路改版 — Case Study 二级页
├── ziruim-app.html         # 自如 APP 首页全链路升级 — 项目详情页
├── assets/
│   ├── work-aigc.jpg       # Works 模块封面图
│   ├── work-ziruim.jpg
│   ├── work-hmi.jpg
│   ├── work-chongbaihui.jpg
│   ├── work-dashboard.jpg
│   └── yihuan/             # 自如 APP 项目素材（PDF 提取并压缩）
│       └── page_1~10.jpg
└── .gitignore
```

## 🎨 设计语言

| 元素 | 规格 |
|---|---|
| 主背景 | `#08080a` |
| 卡片背景 | `#111115` |
| 主色 | 紫粉橙渐变 `linear-gradient(135deg, #a855f7, #ec4899, #f97316)` |
| 强调紫 | `#c084fc`（标题 hover） |
| 荣誉金 | `#fbbf24`（星标徽章） |
| 字体 | Inter（正文）/ JetBrains Mono（标签） |

## 🛠 技术栈

- **HTML5 + CSS3**（无框架依赖）
- **Vanilla JavaScript**（光标动画、滚动揭示、移动端菜单）
- **PyMuPDF + Pillow**（PDF 素材提取与图片压缩）

## 🚀 本地运行

无需构建，直接用任意静态服务器打开即可：

```bash
# Python
python -m http.server 8000

# 或 Node
npx serve
```

然后访问 `http://localhost:8000`。

## 📦 部署

网站已通过 **GitHub Pages** 部署，自动从 `main` 分支根目录构建：

👉 **https://guyinge.github.io/uiux-portfolio/**

每次推送到 `main` 分支会自动触发重新部署。

## 📝 作品模块

| 项目 | 类型 |
|---|---|
| AIGC 辅助设计 | AI Workflow / Creative Tech |
| [自如链路改版](https://guyinge.github.io/uiux-portfolio/ziruim-app.html) | UX Redesign / Product |
| HMI 设计提案 | Interface / Automotive |
| 宠百汇 APP | E-commerce / Mobile |
| 后台系统 & C4D | Dashboard / 3D Visual |

## 📄 License

MIT © LEI · GUYINGE

---

Crafted with passion · Designed for impact
