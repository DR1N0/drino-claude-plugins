# DR1N0 Claude Plugins / DR1N0 Claude插件库

Personal plugin/skill library for Claude Code - Professional tools for AI-assisted development and content creation.

Claude Code的个人插件库 - 用于AI辅助开发和内容创作的工具。

---

## Overview / 概述

This marketplace contains custom skills designed to enhance Claude Code's capabilities for specific workflows. Each skill provides specialized, interactive assistance for complex tasks.

本市场包含为特定工作流程设计的自定义技能，以增强Claude Code的能力。每个技能为复杂任务提供专业的交互式辅助。

---

## Available Plugins / 可用插件

### 🎨 Prompt Generation - AI Content Prompts

**English:** AI prompt generation for creative content including video storyboards, image prompts, and more. Helps you craft optimized prompts for various AI generation tools (Seedance, Midjourney, DALL-E, etc.).

**中文:** 创意内容的AI提示词生成，包括视频分镜、图像提示词等。帮助您为各种AI生成工具（Seedance、Midjourney、DALL-E等）制作优化的提示词。

**Current Skills / 当前技能:**
- 🎬 **Storyboard** - Video AI storyboard generation
  - Bilingual support (English/Chinese)
  - Interactive workflow
  - Optimized for Seedance 2.0, Runway ML, Pika

**Future Skills / 未来技能:**
- 📸 Photo prompts (Midjourney, DALL-E)
- 🎵 Music prompts (Suno, Udio)
- ✍️ Text prompts (creative writing)

[View Documentation](plugins/prompt-gen/README.md)

**Trigger Phrases:**
- English: "Create a storyboard", "generate video prompts", "plan video scenes"
- 中文: "创建分镜", "生成视频提示词", "规划视频场景"

---

## Installation / 安装

1. Add the marketplace / 添加市场:
   ```bash
   /plugin marketplace add DR1N0/drino-claude-plugins
   ```

2. Install the plugin / 安装插件:
   ```bash
   /plugin install prompt-gen@drino-claude-plugins
   ```

3. Restart Claude Code / 重启 Claude Code

---

## Usage / 使用方法

Skills are automatically loaded by Claude Code. Simply mention what you want to do, and Claude will activate the appropriate skill.

技能会被Claude Code自动加载。只需说明您想做什么，Claude就会激活相应的技能。

**Examples / 示例:**

```
# English
"Create a storyboard for my 30-second product video"

# 中文
"为我的30秒产品视频创建分镜脚本"
```

---

## Skill Structure / 技能结构

Each skill in this marketplace follows the official Claude Code plugin structure:

```
plugins/
└── skill-name/
    ├── .claude-plugin/
    │   └── plugin.json       # Plugin metadata
    ├── skills/
    │   └── skill-name/
    │       ├── SKILL.md      # Main skill prompt
    │       ├── references/   # Detailed documentation
    │       └── examples/     # Example workflows
    └── README.md             # Skill documentation
```

---

## Development / 开发

### Adding New Skills / 添加新技能

1. Create plugin directory: `plugins/your-skill/`
2. Add plugin manifest: `.claude-plugin/plugin.json`
3. Create skill: `skills/your-skill/SKILL.md`
4. Update marketplace.json
5. Test with Claude Code

See [Claude Code Plugin Development Guide](https://docs.anthropic.com/claude/docs/plugins) for details.

---

## Requirements / 要求

- Claude Code CLI (latest version)
- Supported platforms: macOS, Linux, Windows

---

## Contributing / 贡献

This is a personal skill library. If you have suggestions or find issues:

1. Open an issue in the repository
2. Describe the problem or enhancement
3. Include examples if applicable

这是个人技能库。如果您有建议或发现问题：

1. 在仓库中创建issue
2. 描述问题或增强建议
3. 如适用，请包含示例

---

## Roadmap / 路线图

**Planned Skills / 计划中的技能:**

- 📝 **Technical Writing** - Documentation and API reference generation
- 🧪 **Test Generator** - Comprehensive test suite creation
- 🎨 **UI/UX Review** - Interface and user experience analysis
- 📊 **Data Visualization** - Chart and graph creation workflows
- 🌐 **i18n Helper** - Internationalization and localization assistant

---

## Version History / 版本历史

### v1.0.0 (2024-02-12)
- Initial release
- Added Prompt Generation plugin with Storyboard skill (bilingual)
- Complete marketplace structure
- Documentation and examples
- Scalable architecture for future prompt generation skills

---

## License / 许可证

MIT License

Copyright (c) 2024 DR1N0

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

## Author / 作者

**DR1N0**

Skills designed for professional AI-assisted workflows.

为专业AI辅助工作流程设计的技能。

---

## Feedback / 反馈

Questions, suggestions, or issues?

问题、建议或问题反馈？

- GitHub Issues: [Create an issue](../../issues)
- Documentation: See individual skill README files

---

**Note:** This skill library is independently maintained and not officially affiliated with Anthropic or Claude.

**注意:** 此技能库为独立维护，与Anthropic或Claude无官方关联。
