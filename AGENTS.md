# MyAgentSkills

这是用户的全局 skills 目录，用于存储和管理用户的自定义 skills。

# 语言规范
自建 skill 的描述必须使用中文，但专业术语保持英文。

# Skill创建的流程
1. 在当前目录创建一个新的目录，目录名就是 skill 名称。
2. 在新目录中创建 `SKILL.md` 文件，用于描述 skill 的功能、使用场景、操作步骤等。
3. 在 `SKILL.md` 文件中添加必要的代码示例、注释等。
4. 保存 `SKILL.md` 文件。
5. 去根目录的 `README.md` 文件，添加新的 skill 名称到 `## 现有 skills` 部分。

# 针对 Trae 全局内存仓库的说明

此目录 (`/Users/zytwd/.trae-cn/skills/`) 是用户的全局 skills 目录，会被所有支持 Trae 的 IDE/编辑器调用。

- **AGENTS.md**: 适用于所有 Trae 兼容 IDE 的全局配置说明
- **skills 目录结构**: 包含具体的 skill 实现，每个 skill 是一个独立目录

如果你正在配置 Trae 的全局 skills 目录，请遵循以上创建流程。
