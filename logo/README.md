> ## ✅ 2026-11-07 再次定稿：以 `hand/` 为准
>
> 业主当日晚确认：以「颜色边界密集取点 → 轻平滑 → 贝塞尔重建」的**手工重绘版**作为公司官方 logo，
> 已替换 yellowfir.com（commit `efdc2c6`）。
>
> - 权威矢量：`hand/yellowfir-{icon,logo-horizontal,logo-vertical}-{color,mono,reverse,on-dark}.svg`
> - 画布：图标 506.59²、横向 1158.59×422.59、竖向 746.59×590.59
> - 指标：871 控制点、100% 曲线段、与源位图 IoU 0.9681
> - 线上副本：`Yellowfir-work/website-Yellowfir/logo/svg/`
> - 本文件下方描述的 `svg/`（potrace 描摹）保留为历史对照，**不再作为交付件**

# Yellowfir 官方标志资产 · 20261107

**这是 Yellowfir Group Limited 的官方标志版本。此前所有版本作废。**

| 项 | 内容 |
|---|---|
| 单号 | D-202611-008 |
| 定版日期 | 2026-11-07 |
| 唯一权威源 | `/Users/john/Desktop/AIfolder/Yellowfir-work/yellowfir Logo.af`（业主 2026-11-07 指定） |
| 矢量取自 | 同目录 `yellowfir Logo.svg`（Affinity 3.3.3 导出，`viewBox="0 0 7200 10800"`，3,781,484 字节） |
| 依据 | 业主原话「之前做的 yellowfir 图标是错误的，要以这个文件为准」 |
| 规范 | 本目录 `品牌规范.md` |
| 生成脚本 | `tools/build.py`（幂等，可随时重跑） |

## 目录

```
_official/
├── 品牌规范.md                     # 构成/留白/最小尺寸/色值/错误用法/切片坐标/命名
├── README.md                       # 本文件
├── 自检记录.md                     # 交付前自检（数字/结构/机器门禁）
├── svg/                            # 10 个矢量文件（全部转曲，无 <text>、无外链）
├── png/                            # 50 个位图（图标 16–1024；锁定 256–2048）
├── favicon.ico                     # 16(micro) + 32(micro) + 48(标准)
├── apple-touch-icon-180.png        # 180×180 白底
├── figures/anatomy.png             # 留白与构成示意图
├── screens/                        # 验收截图 + 可重跑的 HTML
└── tools/{build.py,verify.py}       # 生成脚本 + 机器门禁
```

## 取哪一个

| 场景 | 文件 |
|---|---|
| 页眉 / 邮件签名 / 横位 | `svg/yellowfir-logo-horizontal-color.svg`（深底用 `-reverse`） |
| 页脚 / 封面 / 窄栏 | `svg/yellowfir-logo-vertical-color.svg` |
| 头像 / 应用图标 | `svg/yellowfir-icon-color.svg`；≤32 px 用 `yellowfir-icon-micro-color.svg` |
| 单色印刷（一色） | `svg/yellowfir-logo-*-mono.svg` |
| 深色底 | `svg/yellowfir-logo-*-reverse.svg`（金冠 + 白干 + 白字） |

## 三条最容易被做错的事

1. **树是描摹件**。`.af` 内该对象是位图（导出 SVG 里为 398×290 的 `<use href="#_Image5">`），本体系用 potrace 描摹成矢量，与源位图逐像素 IoU **0.9999**。形状忠实，但若日后拿到原生矢量应替换（见规范 §十一）。
2. **深底不能直接用彩色版**。绿干对深绿底 `#284F34` 仅 **1.31:1**，树干会消失。深底一律 `-reverse`。
3. **16 px 必须用 micro**。标准版在 16 px 冠内镂空塌陷、树干仅 1 px；micro 把标志占比提到 92% 并闭合了冠内空隙。

## 版本关系

- **本目录（20261107）＝ 官方版**。
- `../yellowfir-logo-20261105/` —— **历史版本，已被 20261107 取代**。按业主 2026-11-07 指示，该版本图标「是错误的」，不得再用于任何对外物料；目录原样保留以备追溯，未删除、未改动。
- 站点上现用的 `New yellowfir Logo (WhiteText+blueTrunk) .png` 系列亦属被取代版本。

## 对外使用

对外正式物料发布前须经决策人确认。商标注册用的图形请使用原生矢量源（本描摹件不适用于商标图形提交）。
