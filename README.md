# youqishan.github.io

个人主页 + 网页备忘录，由 GitHub Pages 托管，访问地址：https://youqishan.github.io/

## 目录结构

```
├── index.html        主页（备忘录风格）
├── memos.js          主页「最近备忘」的数据源，编辑它即可增删备忘
├── favicon.svg       站点图标
├── my_work/          日记月历与日记阅读器
├── study/            课程笔记列表与阅读器
├── travel-map/       旅行地图编辑器（Vite 构建产物，直接部署）
└── _config.yml       GitHub Pages 的 Jekyll 配置（本站实际由 .nojekyll 跳过 Jekyll）
```

## 本地预览

```bash
# 任选其一
python3 -m http.server 8000
npx serve .
```

然后打开 http://localhost:8000 。

## 修改旅行地图编辑器后重新构建

源码位于仓库外的工作区目录 `旅行地图编辑器/travel-map/`：

```bash
cd 旅行地图编辑器/travel-map
npm install        # 首次
npm run build      # 产物输出到 dist/
rm -rf ../youqishan.github.io/travel-map
cp -r dist ../youqishan.github.io/travel-map
```

之后按交付指南提交并推送到 GitHub 即可。

## 数据说明

- 旅行地图编辑器的所有数据保存在浏览器 localStorage，导出 ZIP 可备份、可分享；
- 主页备忘为纯文本数据，写在 `memos.js` 里，不涉及隐私。
