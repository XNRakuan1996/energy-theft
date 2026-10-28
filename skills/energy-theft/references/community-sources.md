# 开源社区检索路线

按任务缺口选择渠道；这不是依赖或安装清单。各站点内容、可用性、许可和接口以当时核验为准。

- [GitHub](https://github.com/)：发现完整项目、库、组件和失败经验，追到源仓库的代码、版本、测试、许可证、Issues 或修复。
- [skills.sh](https://skills.sh/) 与 [SkillHub](https://skillhub.cn/)：按任务找 Skill，再追溯作者和原始文件；目录、审核标识和热度不能代替当前场景测试。
- 相关维护者文档、社区及领域资料：针对具体环境、版本与失败条件找补充证据。

把需求拆成能力、平台、输入与限制，用中文、英文和同义词查找；反证可以查 unsupported、limitation、failure、regression。不要把不同转载当作独立证据。找到满足硬约束且已验证的候选后停止，不为凑数无限搜索。

设计参考：[Vercel find-skills](https://github.com/vercel-labs/skills/blob/main/skills/find-skills/SKILL.md) 的发现和检索思路；本 Skill 的适配判断、证据分层与验收流程来自本项目的工作方法，不依赖或安装该 Skill。另见 [Agent Skills 格式规范](https://agentskills.io/specification)。

其他设计参考：

- [evaluate-existing-solutions](https://github.com/citypaul/.dotfiles/blob/main/claude/.claude/skills/evaluate-existing-solutions/SKILL.md)：按影响选择比较深度，评估采用和维护成本。
- [skill-mining](https://github.com/voodootikigod/skill-mining/blob/main/skill-mining/SKILL.md)：创建前查重，区分无法检索和未找到结果。
- [upskill](https://github.com/yungbose/upskill)：根据实际使用中的失败与反馈判断是否修订。
- [Microsoft SkillOpt 维护者报告](https://microsoft.github.io/SkillOpt/blog/gating-reflection-safe-updates/)：将反馈归因、更新和后续验证分开。

这些是方法参考，不代表已安装、运行或整体采用上述项目，也不代表其作者背书本 Skill。具体版本和适用性须在使用时核验。
