# deepsearch

为 agent 提供真正的联网信息检索：本地 SearXNG 聚合多引擎（返回标题/URL/摘要/时间），支持新闻、时间范围、指定引擎；并提供网页正文抽取与「搜索+读前K篇」的深检索

HologramAgent 插件，随 SDK `1.1.2` 的示例插件拆分而来。

## 构建

```bash
hmapdev build
```

产物 `dist/deepsearch_bundle.hmap` 经 `plugin_install` 安装。

## 自动更新

本仓库地址登记在 `plg.json` 的 `repo` 字段，安装后随产物写入
`plugin.json` 的 `repository` 字段 —— 内核的 `plugin_update` 靠它
从本仓库拉最新源码并重编安装。
