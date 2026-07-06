# Dylign · 美国市场进入策略建议

定制贴纸/标签产品线 · 美国市场进入策略报告（2026 年 7 月）。

## 页面

- **`report.html`** — 主报告网页（响应式，含内嵌交互看板）
- `竞品购买流程交互看板.html` — 12 家竞品购买流程交互看板（作为子页面内嵌于报告）
- `index.html` — 下单原型（核心购买流程）
- `labels-home-care.html` / `labels-food-bev.html` — 垂直标签落地页
- `barcode-generator.html` — Barcode 免费获客工具原型

## 本地预览

```bash
python3 -m http.server 8000   # 然后打开 http://localhost:8000/report.html
```

内嵌 iframe 需通过 HTTP(S) 访问（直接双击打开 `file://` 时部分浏览器会阻止 iframe）。
