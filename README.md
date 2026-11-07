# DSH 插件排错速查（DeepSeek Harness Plugin Troubleshooting）

> 社区 issue 里最高频的 10 个 DSH 插件问题，整理成「现象 → 原因 → 三步解决 → 兜底」。
> 数据来源：dsh-market / dsh-plugin-hub 仓库 87 个 open issue 里的 25 条需求类（2026-11 快照）。
> 本仓库免费可复制使用；内容按 MIT 许可。

## 适用版本

- DeepSeek Harness 0.2.x
- 插件市场 dshmarket 1.7x

## 10 个高频问题

### 1. 装插件报 `untrusted origin`
**原因**：市场只信任白名单来源（官方目录 / npm / 作者 Release 包）。
**解决**：① 确认插件在目录里；② 用目录给的安装命令；③ 升级 dshmarket 再试。
**兜底**：把来源链接贴到 issue 里问。

### 2. 插件描述乱码
**原因**：界面语言/区域设置或目录编码。
**解决**：① 设置 → 语言确认简体中文；② 完全重启 DSH（不是关窗口）；③ 系统区域格式设为中文(简体，中国)。

### 3. 装/更新插件提示 `an Agent could not be held at the maintenance boundary`
**原因**：有常驻会话/机器人任务在跑，宿主不允许运行时改插件。
**解决**：① 先停常驻任务；② 再装；③ 仍不行就退出 DSH 全部进程再装。

### 4. 更新插件失败并回滚：`ERR_MODULE_NOT_FOUND`
**原因**：插件处于热挂载，文件被替换后模块解析失败。
**解决**：① 先停用该插件；② 重启 DSH；③ 再更新（不要热挂载状态下硬更）。

### 5. 顶栏一直显示「1 项变更需重启」但重启也消不掉
**原因**：旧版对随启动加载插件的误判，或手写 patch 行格式不被识别。
**解决**：① 升级 dshmarket；② 确认插件实际是开着的；③ 功能正常可忽略该提示。

### 6. 插件装完不显示 / 像没装
**原因**：装到了别的 profile，或需要刷新/重启。
**解决**：① 确认 profile 一致；② 刷新页面；③ 重启 DSH。

### 7. WebDAV 自动备份必然 401
**原因**：市场不保存密码，重启后拿空密码上传（见 issue #1058）。
**解决**：① 关掉每天自动备份；② 重启后重填密码测一次；③ 或改用本地导出 + 网盘同步。

### 8. 恢复备份后插件只剩一半 / 市场消失
**原因**：恢复中断，profile 半成品状态未回滚（见 issue #1128）。
**解决**：① 停手，先备份 profile 目录；② 用恢复前备份重新导入；③ 市场消失就手改 profile 的 package.json 加回 bundles 后重启。

### 9. 更新/下载插件很慢或超时
**原因**：GitHub 网络波动。
**解决**：① 设置 → 插件配置 → GitHub 加速填一个可用 HTTPS 前缀；② 换 npm 镜像；③ 优先用作者 Release 包安装。

### 10. 卸载后 pnpm 策略里留孤儿条目
**原因**：旧版卸载不清理（见 issue #1093）。
**解决**：① 打开 profile 的 `pnpm-workspace.yaml`；② 删掉已卸载包那一行；③ 重跑 `pnpm install` 确认。

## 通用排查顺序

1. 先升级 dshmarket 和 DSH → 重启。
2. 记录**报错原文**。
3. 在 [dsh-market issues](https://github.com/dsh-market/dsh-market/issues) 搜关键词。
4. 动 profile 文件前先复制备份。

## 附：48 个近期维护中的插件（按 star 与更新筛选）

完整清单（含安装命令、要求 DSH 版本）见 [`picks.md`](./picks.md)。

## 需要更新更全的版本？

本仓库内容会随 issue 更新；如果你想要整理好的完整文档（48 插件 + 版本兼容表 + 报错卡），可以到闲鱼搜「DeepSeek Harness 插件安装与报错排查指导」。

## License

MIT
