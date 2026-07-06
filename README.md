# Dylign · 美国市场进入策略建议

定制贴纸/标签产品线 · 美国市场进入策略报告（2026 年 7 月）。

## 结构

```
index.html               # 📊 报告主页（GitHub Pages 入口，响应式，内嵌交互看板）
board/                   # 竞品购买流程交互看板（作为子页面内嵌于报告）
  index.html
  screenshots/ …         #   看板引用的竞品截图
prototype/               # 配套下单原型（自成一体，可独立浏览）
  index.html             #   下单原型（核心购买流程）
  labels-home-care.html  #   家居个护垂直落地页
  labels-food-bev.html   #   食品饮料垂直落地页
  barcode-generator.html #   Barcode 免费获客工具原型
  assets/ …              #   原型的 CSS 与图片
```

- **报告** → `/`（即 `index.html`）
- **交互看板** → `/board/`
- **下单原型** → `/prototype/`

## 本地预览

```bash
python3 -m http.server 8000   # 然后打开 http://localhost:8000/
```

内嵌 iframe 需通过 HTTP(S) 访问（直接双击 `file://` 打开时部分浏览器会阻止 iframe）。

## GitHub Pages

已启用 Pages（master 分支根目录）。部署后报告地址为
`https://<用户名>.github.io/dylign-market-entry-report/`。
