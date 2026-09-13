# Qiyuan Zhuang · 庄启源

个人学术主页，基于原生 HTML / CSS / JavaScript，直接兼容 GitHub Pages，无需安装依赖或构建。

## 本地预览

在仓库目录运行 `python3 -m http.server 8000`，访问 http://localhost:8000。

## 内容维护

- `index.html`：个人介绍、论文、经历、教育背景、荣誉与联系方式。
- `style.css`：排版、颜色和移动端布局。
- `script.js`：滚动时高亮导航、更新页脚年份。
- `resource/`：现有获奖证书与技术报告；保留原有链接。

页面以 `cv-zh` 简历为内容来源；在审与已发表 / 已录用论文分开展示。字体使用 Google Fonts，无法加载时自动回退到系统字体。

## GitHub Pages

将更改提交并推送至 GitHub 后，在仓库 Settings → Pages 中选择 Deploy from a branch，选择网站所在分支与 `/ (root)`。发布地址为 https://watereand.github.io/ 。如果仓库已经配置 Pages，沿用现有发布设置即可。

## 论文配图

参考 https://jiayuanm.com/ 的学术主页布局，采用紧凑的个人介绍与左图右文论文列表。

6 篇论文都在 HTML 中预留了 `figure.paper-figure`，桌面宽 260px，默认比例 8:5；手机端图片排列在文字上方。没有图片时显示浅色占位区域，不请求不存在的图片。

把图片放到 `resource/papers/`，然后在对应论文的 `figure` 中删除 `div.figure-placeholder`，取消已经写好的 `img` 注释即可。推荐 720×450 或更高分辨率，图片使用 contain 完整展示，不裁剪图中内容。

| 论文                 | 建议图片名               |
| -------------------- | ------------------------ |
| RAAP                 | raap.png                 |
| LeaP                 | leap.png                 |
| Coarse Labels Matter | coarse-labels.png        |
| Quantum-Inspired VPT | quantum-prompt.png       |
| Temporal Uncertainty | temporal-uncertainty.png |
| Undergraduate Thesis | thesis.png               |
