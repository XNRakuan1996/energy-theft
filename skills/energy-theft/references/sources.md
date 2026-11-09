# 来源与设计边界

作者：阿宽（AKuan）。本文件记录公开的方法来源与取舍；当前任务的查询、入口、转向与停止条件见[查找方法](community-sources.md)。来源引用不是安装要求，也不授权额外访问、执行或外发。

## 公开方法来源

| 来源 | 借用的思路 | 未沿用的部分与边界 |
| --- | --- | --- |
| [Agent Skills 格式规范](https://agentskills.io/specification) | SKILL.md 前言、目录命名与按需引用 | 格式符合不保证任何宿主自动兼容或加载 |
| [Vercel find-skills](https://github.com/vercel-labs/skills/blob/main/skills/find-skills/SKILL.md) | 按能力与领域发现现成 Skill，再追到原始仓库 | 不把安装量或星标当适用性证明，不自动安装 |
| [citypaul evaluate-existing-solutions](https://github.com/citypaul/.dotfiles/blob/main/claude/.claude/skills/evaluate-existing-solutions/SKILL.md) | 比较采用后的总成本，用证据决定复用或新建 | 不引入作者的整套依赖、能力路由或审批流程 |
| [voodootikigod skill-mining](https://github.com/voodootikigod/skill-mining/blob/main/skill-mining/SKILL.md) | 创建前查重，区分检索不可用与没有结果，避免旧验证冒充当前验证 | 不复制其评分和多代理流程，不运行其 CLI |
| [yungbose/upskill](https://github.com/yungbose/upskill/blob/main/upskill/SKILL.md) | 提炼成功与纠错，把待验证候选和已固化方法分开 | 在原任务保留反馈，不复制次数阈值或跨 Skill 扩散机制 |
| [Microsoft SkillOpt 维护者报告](https://microsoft.github.io/SkillOpt/blog/gating-reflection-safe-updates/) | 区分方法缺陷与执行遗漏，保留验证、检查点和回退 | 不套用研究阈值、模型/API或夜间运行方式，不移植研究收益数字 |
| [Anthropic skill-creator](https://github.com/anthropics/skills/blob/main/skills/skill-creator/SKILL.md)及[匿名比较方法](https://github.com/anthropics/skills/blob/main/skills/skill-creator/agents/comparator.md) | 固定输入与工具，先看产物再评价，保留未参与修改的任务 | 允许结果相同；不强求分胜负，不把反复用于调优的样本当最终效果证明 |

## 本 Skill 的适配

将现有发现方法与按约束选择方案的方法组合：先按第一性原理明确目标、事实和硬约束，再生成查询，依据实际结果选择继续查找、验证、复用、组合或只补缺口，最后验收真实交付。

借鉴的是工作方法，没有复制或执行上述项目的实现、安装器或评测脚本。本 Skill 不新增搜索引擎、外部服务或后台训练平台；实际工具能力、登录状态、费用和权限由当前运行环境决定。

原始仓库和报告可能更新，使用时核对当前版本与适用条件。链接仅定位来源，不代表来源作者为本 Skill 背书；引用不等于获得整套第三方内容的复制与分发权限，实际使用仍须核对相应许可。

## 验证边界

格式检查、示例运行和具体任务成功分别说明不同事实，不等同于跨任务提效。一次重放、一次调用或局部对照不能证明稳定减少重复工作、返工和用户纠偏；没有对应证据时保留未知，不声称长期收益。
