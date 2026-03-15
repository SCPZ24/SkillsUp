---
name: 创建SKILL
description: 当用户需要创建新的skill时，参考此skill的指导步骤。
---

# 创建SKILL
name: create-skill
description: 提供创建新skill的完整流程和模板，帮助用户快速创建符合规范的skill
type: guide
version: 1.1
author: Trae User

## 核心指令（创建步骤）
instructions:
  ### 步骤 1：创建目录结构
  1.1 在当前目录(trae的全局skill目录)下创建一个新的目录，目录名就是 skill 名称。
  1.2 目录名建议使用中文，清晰表达skill的功能。
  
  ### 步骤 2：创建 SKILL.md 文件，注意用中文！
  2.1 在新目录中创建 `SKILL.md` 文件。
  2.2 文件必须包含以下结构：
     - Banner 部分（YAML front matter）
     - 详细描述部分
     - 核心指令/步骤
     - 输出模板（如有）
  
  ### 步骤 3：编写 Banner 部分
  3.1 在文件开头添加 YAML front matter：
  ```yaml
  ---
  name: skill名称（中文）
  description: skill的功能描述
  ---
  ```
  
  ### 步骤 4：编写详细内容
  4.1 包含：
     - 技能名称（英文和中文）
     - 详细描述
     - 核心指令/步骤
     - 依赖工具（如有）
     - 输出模板（如有）
  
  ### 步骤 5：更新 README.md
  5.1 打开 `README.md` 文件
  5.2 在 `## 现有 skills` 部分添加新的 skill 名称
  
  ### 步骤 6：验证和测试
  6.1 检查文件结构是否正确
  6.2 确保所有内容符合语言规范
  6.3 测试 skill 是否能被正确识别

## 语言规范
- 自建 skill 的描述必须使用中文，但专业术语保持英文
- 文件名和目录名使用中文，便于理解
- 代码示例和技术术语使用英文

## 依赖工具（可选）
tools:
  - filesystem.read  # 读取现有 skill 模板
  - filesystem.write # 创建新的 skill 文件
  - terminal.run     # 执行命令创建目录结构

## 输出模板（SKILL.md 模板）
output_template: |
  ---
  name: {skill名称（中文）}
  description: {skill的功能描述}
  ---

  # {skill名称（中文）}
  name: {skill名称（英文）}
  description: {详细描述}
  version: 1.0
  author: Trae User

  ## 核心指令
  instructions:
    ### 步骤 1：{步骤描述}
    {详细内容}

    ### 步骤 2：{步骤描述}
    {详细内容}

  ## 依赖工具
  tools:
    - {工具名称}  # {用途说明}

  ## 输出模板
  output_template: |
    {输出格式模板}