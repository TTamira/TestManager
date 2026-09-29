# Changelog

本项目所有可追踪变更均登记于此，遵循 [Keep a Changelog](https://keepachangelog.com/) 约定。
变更类型：**新增 / 修复 / 变更 / 移除**。

## 留痕约定（四层）
1. **Commit**：Conventional Commits + 中文主题；正文强制包含 `变更说明 / 影响范围 / 关联问题`。
2. **本文件（CHANGELOG）**：每次改动在 `[Unreleased]` 下对应分类登记，注明日期与提交短哈希，是改动清单主入口。
3. **代码行内标记**：缺陷修复处留 `// [FIX-YYYYMMDD-NN] 原因与做法`，与本条 CHANGELOG 一一对应。
4. **分支与 tag**：`main` 只收可运行版本；改动走 `feat/xxx`、`fix/xxx`；里程碑打 `vX.Y.Z` tag。

---

## [Unreleased]

## [0.1.0] - 2026-09-29
### 新增
- 测试用例管理系统（ONES 对齐）设计方案 v0.1：`ONES对齐测试用例管理系统_设计方案_v0.1.html`
  - 调研 ONES 测试用例管理模型：层级主干、字段体系（原子字段 / 字段配置解耦）、形态（文本型 / 步骤型）、测试计划与执行、导入能力现状。
  - 确定 XMind 导入三套可切换识别模式：M1 前缀声明 / M2 标记驱动 / M3 层级推导；明确新版 `.xmind`（XMind 2020+/Zen）真数据在 `content.json` 而非 `content.xml` 的坑点。
  - 确认"执行情况"四态：**通过 / 不通过 / 阻塞 / 待确认**（用户 2026-09-29 指定；系统保留"未执行"初始态，不计入可选四态）。
- 初始化项目版本管理：建立 `D:\TestManager` git 仓库、提交身份（local）、`.gitignore`、本 `CHANGELOG.md`。
