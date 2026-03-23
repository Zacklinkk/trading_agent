# Trading Agent

AI 驱动的行业研究与投资分析工具，当前通过 GitHub Pages 对外展示研究报告与财报分析入口。

## 在线 Pages

- GitHub Pages 地址：<https://zacklinkk.github.io/trading_agent/>
- 发布来源：`main` 分支根目录
- 首页文件：`index.html`

## 为什么在仓库网页里看不到“Pages”

GitHub Pages 是 GitHub 的发布能力，不会在仓库文件树里额外出现一个叫“Pages”的目录。

这个仓库当前的发布方式是：

- Branch: `main`
- Folder: `/`（仓库根目录）

所以真正控制首页内容的文件，就是仓库根目录下的 `index.html`。

## 目录结构

- `index.html`
  Pages 首页，负责展示报告入口、筛选和在线阅读入口。
- `reports/manifest.json`
  报告索引清单，首页会读取它来生成卡片和统计信息。
- `reports/*.html`
  具体研究报告或财报分析页面。

## 当前收录报告

| 报告 | 行业 | 公司 | 代码 |
|------|------|------|------|
| [崇达技术研究报告](reports/崇达技术_研究报告_图表.html) | PCB（印制电路板） | 崇达技术 | 002815.SZ |
| [神州信息研究报告](reports/神州信息_研究报告_图表.html) | IT 服务 | 神州信息 | 000555.SZ |
| [国睿科技研究报告](reports/国睿科技_研究报告_图表.html) | 国防军工（雷达电子） | 国睿科技 | 600562.SH |
| [国睿科技财报分析](reports/国睿科技_财报分析报告.html) | 国防军工（雷达电子） | 国睿科技 | 600562.SH |

## 本地预览

在仓库根目录启动一个静态文件服务即可：

```bash
python -m http.server 8000
```

然后打开：

```text
http://localhost:8000/
```

## 报告特点

- 生命周期驱动分析：结合行业阶段动态调整分析重点。
- 结构化框架：覆盖行业概览、护城河评估、竞争格局、PEST 与估值。
- 交互式图表：支持 tooltip、缩放等交互操作。
- 数据驱动：基于公开金融数据与行业研究信息整理生成。

## License

MIT
