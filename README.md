# DR1N0 Claude Plugins / DR1N0 Claude插件库

Personal plugin/skill library for Claude Code - Professional tools for AI-assisted development and content creation.

Claude Code的个人插件库 - 用于AI辅助开发和内容创作的工具。

---

## Overview / 概述

This marketplace contains custom skills designed to enhance Claude Code's capabilities for specific workflows. Each skill provides specialized, interactive assistance for complex tasks.

本市场包含为特定工作流程设计的自定义技能，以增强Claude Code的能力。每个技能为复杂任务提供专业的交互式辅助。

---

## Available Plugins / 可用插件

### 🎨 Prompt Generation - Seedance 2.0 Video Prompts

**English:** Specialized AI prompt generator for **Seedance 2.0** (ByteDance's video AI). Automatically splits your video ideas into 3-4 independent single shots that can be generated separately and stitched together. Understands Seedance's unique single-shot architecture.

**中文:** 专为**Seedance 2.0**(字节跳动视频AI)设计的提示词生成器。自动将您的视频想法拆分成3-4个独立单镜头，可分别生成后拼接。深度理解Seedance的单镜头架构。

**Current Skills / 当前技能:**
- 🎬 **Seedance Shots** - 单镜头组生成器 (v1.0)
  - Single-shot splitting logic / 单镜头拆分逻辑
  - Interactive AskUserQuestion workflow / 交互式问答
  - Chinese-first strategy / 中文优先策略
  - Multi-modal references / 多模态引用
  - Video extension & editing / 视频延长和编辑

**Why Seedance-focused? / 为什么专注Seedance?**
- Traditional storyboards use timeline control (0-3s, 3-7s) - doesn't work with Seedance
- Seedance is a single-shot model - needs independent shots, not multi-scene scripts
- Deep platform optimization beats generic solutions

**Future Skills / 未来技能:**
- 📸 Seedance Image (image-to-video)
- 🎵 Music Sync (beat-matching)
- 🎬 Long-form Narrative (30s+ stories)

[View Documentation](plugins/prompt-gen/README.md)

**Trigger Phrases:**
- English: "Create video shots for...", "Generate Seedance prompts", "Make a video about..."
- 中文: "帮我生成...的视频镜头", "创建Seedance提示词", "制作关于...的视频"

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
└── plugin-name/
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

1. Create plugin directory: `plugins/your-plugin/`
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

### v1.0.0 (2024-02-13)
- Major refactor: Generic storyboard → Seedance 2.0 specialized
- Renamed skill: storyboard → seedance-shots
- Single-shot splitting logic (matches Seedance architecture)
- Interactive AskUserQuestion workflow
- Chinese-first language strategy
- 10+ comprehensive examples
- Quick reference, technical specs, templates
- Multi-modal reference support
- Video extension and editing features

### v0.1.0 (2024-02-12)
- Initial release (generic storyboard)
- Deprecated due to platform mismatch

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
