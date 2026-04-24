# Ornn — GPU 界面原型

单文件静态页（`ornn_app.html` 等）+ 资源位图。根路径 `index.html` 会跳转到主应用。

## 仓库

- **GitHub:** [github.com/Xiaoyang-Hu-96/ornn-gpu-prototype](https://github.com/Xiaoyang-Hu-96/ornn-gpu-prototype)

## 在 GitHub Pages 上托管

在 **Settings → Pages** 里选择：

- **Source:** Deploy from a branch  
- **Branch:** `main` / `(root)`  

站点地址形如：`https://xiaoyang-hu-96.github.io/ornn-gpu-prototype/`（以你在 Pages 中看到的实际 URL 为准）  
首页会经 `index.html` 进入 `ornn_app.html`。

## 在 Vercel 上部署

1. 登录 [Vercel](https://vercel.com) → **Add New** → **Project**  
2. **Import** 本 Git 仓库（与 GitHub 已连接时可直接选）  
3. **Framework Preset:** Other；**Build / Output** 留空或默认  
4. **Deploy**  

- **已绑定的生产地址:** [ornn-gpu-prototype.vercel.app](https://ornn-gpu-prototype.vercel.app)（根路径会进入 `index.html` → 主应用）  
- 与 Git 仓库已连接，每次 `git push` 会自动重新部署。

### 访问人数 / 页面浏览（Vercel Web Analytics）

各 HTML 页面已加入官方 [Web Analytics](https://vercel.com/docs/analytics) 脚本，在 **Vercel 控制台开启** 后才会统计访问量：

1. 打开 [Vercel Dashboard](https://vercel.com/dashboard) → 选中本项目 **ornn-gpu-prototype**  
2. 顶部或侧栏进入 **Analytics**（或 **Observability → Web Analytics**）  
3. 点击 **Enable** 开启  
4. **再部署一次**（推一次代码或 Redeploy），之后即可在面板里看到访客、热门页面、来源等（匿名、无 Cookie，[说明见文档](https://vercel.com/docs/analytics/privacy-policy)）  

免费档有每月事件数限制，详见 [Analytics 定价](https://vercel.com/docs/analytics/limits-and-pricing)。本地用 `file://` 打开页面时请求 `/_vercel/insights/script.js` 会失败，属正常现象。

## 本地包含的文件

- `ornn_app.html` — 主应用（导航、市场、预约等）  
- 其他 `ornn_*.html` — 分屏/版本实验页  
- `logo.png`, `logo2.png`, `nvidia.png`, `core.png` — 界面资源  

## 环境说明

- 无需 `npm install` 或构建步骤。  
