# public-share

LeapBound AI 对外分享文件的 GitHub Pages 托管**实验仓**。

线上入口：<https://leapbound-ai.github.io/public-share/>

## 为什么有这个仓

我们现有的分享托管走 `leapbound.ai/share/<slug>`（Cloudflare Pages Function +
Supabase Storage，见团队文档 LB14）。这个仓是拿 GitHub Pages 做同一批文件的
**对照组**，用来实测两条链路的差别：

- 国内网络下的可达性（`github.io` vs 已备案的 `leapbound.ai`）
- 大文件（17.5 MB 单页 HTML）的首屏加载速度
- 微信内置浏览器能否正常打开

## 内容

| 文件 | 说明 |
|---|---|
| `index.html` | 导航页 |
| `flipbook-prod.html` | 手机竖版翻页演示，6 页，17.5 MB（图片内嵌为 base64） |
| `bos-v2.html` | 复利引擎落地页 v2 改稿预览，37 KB |

均为 LeapBound 自有对外物料，与 `leapbound.ai/share/` 上的同名文件一致。

## ⚠️ 这是 public 仓

任何人可访问，且会被搜索引擎与 GitHub 代码搜索索引 —— 与
`leapbound.ai/share/<slug>`「知道 slug 才打得开」的半私密语义**不同**。

**不要**往这里放客户机密、内部成本、未公开的方案或任何含个人信息的文件。
需要控制可发现性的内容，走 `leapbound.ai/share/`。
