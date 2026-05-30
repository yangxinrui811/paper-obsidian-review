# paper-obsidian-review

> 个性化增强版 · 基于 [LiLiXJTU/paper-obsidian-review](https://github.com/LiLiXJTU/paper-obsidian-review) 的 Codex 文献调研技能

## 简介

将论文、代码仓库、本地 PDF 整理为 **Obsidian 结构化中文学术笔记**，支持多课题并行管理、引文网络驱动的文献补齐、批量论文下载、DOI 验证。

## 相比原始版本的增强

| 功能 | 原始版本 | 本版本 |
|---|---|---|
| **文件命名** | 手动随意 | `YYYY-JournalAbbrev-短语描述` 统一规范 |
| **Vault 组织** | 笔记散放根目录 | 按课题分子文件夹，`pdfs/` 和 `attachments/` 根目录共享 |
| **引文补齐** | 无 | 从已有文献引文网络中反向挖掘缺失的奠基性论文 |
| **论文下载** | 手动 | Semantic Scholar / CrossRef / arXiv 批量下载 + DOI 验证 |
| **总览笔记** | 单篇对比 | 增加课题级"文献演化脉络"和"课题定位建议" |
| **链接管理** | 手动 | 重命名时自动批量更新所有 `[[wiki链接]]` |

## 使用示例

```
用户: 读一下这个文献目录，整理成 Obsidian 笔记

技能自动完成:
  1. 扫描目录 → 统一重命名 PDF → 复制到 vault
  2. 提取全文 → 按结构写单篇笔记 → 生成课题总览
  3. 分析引文网络 → 找出缺失论文 → 输出 DOI 清单
  4. 下载可获取的 OA 论文 → 重命名 → 补充笔记
```

## 安装

```bash
# 通过 Codex skill-installer
codex skill install yangxinrui811/paper-obsidian-review
```

或手动复制 `SKILL.md` 到 `$CODEX_HOME/skills/paper-obsidian-review/`。

## 依赖

- `pdfplumber`：PDF 文本提取
- Semantic Scholar API：论文搜索与 OA 下载
- CrossRef API：DOI 验证

## 致谢

本技能基于 [LiLiXJTU/paper-obsidian-review](https://github.com/LiLiXJTU/paper-obsidian-review) 修改，感谢原作者的结构化笔记框架。
