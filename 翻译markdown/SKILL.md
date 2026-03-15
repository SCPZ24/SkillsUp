---
name: 翻译markdown
description: 当用户提到要翻译markdown(或.md文件)为中文时，触发该skill
---

# 翻译markdown

This skill translates markdown (.md) files to Chinese while preserving the original formatting and external references.

## When to Use

- User asks to translate an English .md file to Chinese
- User wants to create a Chinese version of a markdown document
- User references an English .md file and requests translation

## How It Works

1. Read the specified English .md file
2. Translate all text content to Chinese while preserving:
   - Markdown syntax (headers, lists, code blocks, etc.)
   - External references (images, links, etc.)
   - Code blocks and technical terms
3. Create a new file in the same directory with the naming convention: `{original_filename}_CN.md`

## Usage Example

If the user asks: "Translate the README.md file to Chinese"

You should:
1. Read the README.md file
2. Translate the content to Chinese
3. Create README_CN.md in the same directory with the translated content

## Important Notes

- Preserve all markdown formatting exactly
- Keep external references (images, links) unchanged
- Do not translate code blocks, technical terms, or proper nouns
- Maintain the original file structure and hierarchy