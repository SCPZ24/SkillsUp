# SkillsUp

这是我的个人 Agent Skills 仓库。

大家可以通过这个仓库快速入门skills，并参考我用的skills来设计自己的skills。

## IDE如何调用skills？
以Trae CN为例，ide会把skills放在/trae-cn/skills目录下。

结构为/skill_name/SKILL.md

SKILL.md的banner里添加名称(name)和调用条件(description)。后面用文字表述skill的具体内容（流程等）。

IDE会自动识别，并把skill描述信息加进agent调用的上下文。在用户涉及到可能用得到skill需求时，IDE会自动呼出skill的具体内容填入prompt。

## 安装方法

将此仓库克隆到你的Trae(或其他IDE)的全局 skills 目录：

```bash
git clone https://github.com/SCPZ24/MyAgentSkills.git ~/.trae-cn/skills
```

克隆后，你就可以在 Trae 中使用这些 skills 了。

## 现有 skills

- git提交
- 源码架构快速解析
- 创建SKILL
