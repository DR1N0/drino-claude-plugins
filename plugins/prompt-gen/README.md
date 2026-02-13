# Prompt Generation Plugin / AI提示词生成插件

AI prompt generation for creative content including video storyboards, image prompts, and more.

创意内容的AI提示词生成，包括视频分镜、图像提示词等。

---

## Overview / 概述

This plugin provides AI prompt generation skills for various creative content types. Currently includes video storyboarding, with future support for image, music, and text prompts.

此插件为各种创意内容类型提供AI提示词生成技能。目前包括视频分镜，未来将支持图像、音乐和文本提示词。

## Current Skills / 当前技能

### 🎬 Storyboard - Video AI Prompts

**English:** Create professional storyboards for video AI generation tools (Seedance 2.0, Runway ML, Pika).

**中文:** 为视频AI生成工具（Seedance 2.0、Runway ML、Pika）创建专业分镜脚本。

**Features / 功能:**
- ✨ Bilingual support (English/Chinese) / 双语支持
- 🎬 Interactive step-by-step workflow / 交互式逐步工作流
- 🤖 AI-optimized prompts / AI优化提示词
- 📋 Multiple export formats / 多种导出格式
- 🎨 Camera, lighting, and mood guidelines / 摄影、灯光和情绪指南

## Future Skills / 未来技能

- 📸 **Photo Prompt** - Image generation prompts for Midjourney, DALL-E, Stable Diffusion
- 🎵 **Music Prompt** - Music generation prompts for Suno, Udio
- ✍️ **Text Prompt** - Creative writing and content generation prompts

---

## Installation / 安装

1. Clone or download this skill library to your local machine:
   ```bash
   git clone <your-repo-url> ~/.claude/plugins/marketplaces/drino-claude-skills
   ```

2. Reload Claude Code plugins or restart Claude Code

3. The prompt-gen plugin and its skills will be automatically discovered and available for use

---

## Usage / 使用方法

### English Triggers

Activate the skill by asking Claude:
- "Create a storyboard for a 30-second commercial"
- "Help me plan video scenes for a product demo"
- "I need a storyboard for my short film"
- "Generate video prompts for Seedance"

### 中文触发词

通过以下方式激活技能：
- "创建一个30秒广告的分镜脚本"
- "帮我规划产品演示视频的场景"
- "我需要为短片创建分镜"
- "为Seedance生成视频提示词"

---

## Example Workflow / 工作流示例

### English Example

```
User: Create a storyboard for a 30-second coffee commercial

Claude: Great! Let's create a storyboard for your coffee commercial.

Project Details:
- Duration: 30 seconds
- Purpose: Commercial

Let me ask a few questions:
1. What's the overall mood? (e.g., cozy morning, energetic, luxury)
2. What's the key message or selling point?
3. Any specific settings? (café, home kitchen, nature)

[Interactive conversation continues...]

[Claude generates complete storyboard with:
- Scene-by-scene breakdown table
- AI-ready prompts for each scene
- Technical notes and recommendations]
```

### 中文示例

```
用户: 创建一个30秒咖啡广告的分镜脚本

Claude: 好的！让我们为您的咖啡广告创建分镜脚本。

项目详情：
- 时长：30秒
- 用途：广告

让我问几个问题：
1. 整体情绪是什么？(例如：温馨早晨、充满活力、奢华)
2. 关键信息或卖点是什么？
3. 有特定场景吗？(咖啡馆、家庭厨房、自然环境)

[交互对话继续...]

[Claude生成完整分镜脚本包括：
- 逐场景分解表格
- 每个场景的AI就绪提示词
- 技术说明和建议]
```

---

## What Gets Generated / 生成内容

### 1. Storyboard Table / 分镜表格

| Scene | Duration | Visual Description | Camera | Mood | Transition |
|-------|----------|-------------------|---------|------|------------|
| 1     | 5s       | Coffee beans pouring into grinder | ECU, slow-mo | Anticipation | Match cut |
| 2     | 4s       | Steam rising from brewing coffee | MS, tilt up | Aromatic | Dissolve |
| ...   | ...      | ...               | ...     | ...  | ...        |

### 2. AI-Ready Prompts / AI就绪提示词

```
Scene 1: 5s

Extreme close-up of dark brown coffee beans being poured into a
sleek ceramic grinder, shot in slow motion. Warm morning light
highlights the glossy surface. Shallow depth of field.

Keywords: coffee beans, slow motion, ECU, warm lighting, premium
```

### 3. Technical Specifications / 技术规格

- Resolution recommendations
- Aspect ratio suggestions
- Color palette notes
- Audio suggestions
- Platform-specific optimizations

---

## Reference Documentation / 参考文档

The plugin includes comprehensive guides:

### [Workflow Guide](skills/storyboard/references/workflow-guide.md)
Complete reference for:
- Camera terminology (English + 中文)
- Lighting techniques
- Mood and atmosphere guidelines
- Color palette recommendations
- Platform-specific tips (Seedance, Runway, Pika)
- Prompt engineering best practices

### [Examples](skills/storyboard/examples/)
Ready-to-use storyboard templates:
- [30-second commercial](skills/storyboard/examples/commercial-30s.md) - Coffee brand ad
- [60-second short film](skills/storyboard/examples/short-film-zh.md) - Emotional narrative (中文)

---

## Supported Video Types / 支持的视频类型

- **Commercials / 广告** (15-30s)
- **Social Media Content / 社交媒体内容** (15-60s)
- **Short Films / 短片** (1-5min)
- **Product Demos / 产品演示**
- **Tutorials / 教程**
- **Music Videos / 音乐视频**

---

## AI Platform Optimization / AI平台优化

This skill generates prompts optimized for:

- **Seedance 2.0** - ByteDance's video AI generator
- **Runway ML** - Creative video AI platform
- **Pika** - Fast video generation
- Other text-to-video AI tools

Each platform has specific strengths, and the skill provides tailored recommendations.

---

## Tips for Best Results / 获得最佳效果的技巧

### English
1. **Be specific** - Provide details about mood, style, and message
2. **Think visually** - Describe what viewers should see
3. **Plan transitions** - Consider how scenes flow together
4. **Use references** - Mention specific styles or films for inspiration
5. **Iterate** - Refine prompts based on AI output

### 中文
1. **具体描述** - 提供关于情绪、风格和信息的细节
2. **视觉化思考** - 描述观众应该看到什么
3. **规划转场** - 考虑场景如何衔接
4. **使用参考** - 提及特定风格或电影作为灵感
5. **迭代优化** - 根据AI输出改进提示词

---

## Camera Terminology Quick Reference / 摄影术语快速参考

| English | 中文 | Abbreviation |
|---------|------|--------------|
| Wide Shot | 远景 | WS |
| Medium Shot | 中景 | MS |
| Close-Up | 特写 | CU |
| Extreme Close-Up | 大特写 | ECU |
| Pan | 横摇 | - |
| Tilt | 竖摇 | - |
| Dolly | 移动车 | - |
| Zoom | 变焦 | - |

For complete terminology guide, see [Workflow Guide](skills/storyboard/references/workflow-guide.md).

---

## Contributing / 贡献

This is a personal skill library, but suggestions and improvements are welcome!

这是个人技能库，但欢迎提出建议和改进！

---

## Version History / 版本历史

**v0.1.0** (2024-02-12)
- Initial release
- Bilingual support (English + Chinese)
- Interactive workflow implementation
- Comprehensive reference documentation
- Example templates included

---

## License / 许可证

[Your License Here]

---

## Author / 作者

**DR1N0**

For questions or feedback, please open an issue in the repository.

如有问题或反馈，请在仓库中创建issue。
