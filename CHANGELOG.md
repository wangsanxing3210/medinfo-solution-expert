# Changelog

本文件记录 medinfo-solution-expert 的版本迭代。版本号遵循语义化版本（MAJOR.MINOR.PATCH）。

---

## v1.1.0 — 2026-07-24

**标准时效性重大更新（针对 AI 评分失分修复）**

- **P0 · 电子病历/智慧医疗分级评价标准全面升级**
  - `references/standards.md` 电子病历分级评价章节重写为 2025 版《智慧医疗分级评价方法及标准》
  - 级别由 0-8 级（9 级）调整为 1-8 级；评价指标 779→752 项
  - 新增医疗质量管理、电子病历安全 2 个评价角色（共 12 个）
  - 明确 22 个闭环场景、区域协同（5 级起）、AI 评价 17 项、国产替代/国密要求
  - 数据质量维度由 4 个调整为 5 个（唯一性/完整性/合规性/同一性/时效性）
  - 同步更新 `SKILL.md` 政策检索、模板章节数；`audit-checklist.md` 评级目标与关键节点；`ai-applications.md` 第九章对齐 17 项 AI 评价；`README.md` 场景与知识库描述

- **P0 · 安全合规新增密评/国密要求**
  - `standards.md` 等保章节补充商用密码应用安全性评估（密评）为三级医院评审前置否决项、国密 SM2/SM3/SM4 强制要求
  - `audit-checklist.md` 第五章新增密评与国密检查项
  - 修正事实错误：《医疗卫生机构网络安全管理办法》文号 〔2022〕9 号 → 〔2022〕29 号
  - 数据安全章节补充《医疗卫生机构数据安全和个人信息保护管理办法（试行）》（国卫规划发〔2026〕6 号）

- **P1 · 文档一致性**
  - 修复 `SKILL.md` 章节数自相矛盾（"11 章节"列举 12 个）：统一为"文档摘要 + 11 个正文章节"
  - 精简 `SKILL.md` frontmatter description（650+ 字 → 约 250 字聚焦），触发词保留在触发条件章节
  - 新增"流程示例（Few-shot）"章节，补充编撰/审核/优化三类输入-输出示例

- **P2 · 规范与合规**
  - `SKILL.md` 新增安全与伦理声明（不处理真实患者/隐私数据、脱敏要求）
  - `scenarios.md` 第 315 行交叉引用由"见场景七"改为指向 `references/cloud-prescription.md`
  - 新增 `LICENSE`（MIT）与 `CHANGELOG.md`，README 许可章节引用 LICENSE
  - 版本号 1.0.0 → 1.1.0

---

## v1.0.0 — 2026-07-23

- 初始发布：SKILL.md 编撰/审核/优化三大流程
- references：standards / systems / scenarios（10 大场景）/ ai-applications / audit-checklist / central-pharmacy / cloud-prescription
- assets：solution-template.md（11 章方案模板）
- README.md 对外说明
