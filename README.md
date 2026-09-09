# 百鱼官网 · 上海百鱼电子科技有限公司

"匠心营造 · 品质为本" —— 纯静态企业官网，可直接部署到 GitHub Pages。

## 业务板块

- 土建工程
- 装饰装修
- 加固维修
- 光伏工程
- 宠物相关产品

## 文件结构

```
baiyu-website/
├── index.html        # 首页（公司优势 + 五大板块导航）
├── tujian.html       # 土建工程
├── zhuangshi.html    # 装饰装修
├── jiagu.html        # 加固维修
├── guangfu.html      # 光伏工程
├── chongwu.html      # 宠物相关产品
├── css/style.css     # 全站样式（含响应式）
├── js/main.js        # 交互脚本（导航/回到顶部/入场动画/数字滚动）
├── assets/logo.png   # 公司 Logo
├── robots.txt        # 搜索引擎抓取规则
└── .nojekyll         # 跳过 Jekyll 处理（GitHub Pages）
```

## 本地预览

直接双击 `index.html` 即可在浏览器中打开；或在本目录运行：

```bash
python -m http.server 8000
# 访问 http://localhost:8000
```

## 部署到 GitHub Pages

1. 在 GitHub 新建一个仓库（例如 `baiyu-website`，公开 Public）。
2. 将本目录所有文件推送到仓库：

```bash
git init
git add .
git commit -m "init: 百鱼官网"
git branch -M main
git remote add origin https://github.com/<你的用户名>/baiyu-website.git
git push -u origin main
```

3. 打开仓库 **Settings → Pages**，Source 选择 **Deploy from a branch**，Branch 选择 **main / (root)**，保存。
4. 等待 1-2 分钟，访问 `https://<你的用户名>.github.io/baiyu-website/` 即可。

> 如使用仓库 `用户名.github.io` 作为仓库名，则直接访问 `https://用户名.github.io/`。

## 修改联系方式 / 内容

电话 `021-57475098` 出现在每个页面的顶栏、导航、CTA 区和页脚，全局搜索替换即可。
