# Prompt Generation Plugin / AI提示词生成插件

AI prompt generation for creative video content, specialized for Seedance 2.0 single-shot video generation.

专为Seedance 2.0单镜头视频生成优化的AI提示词生成插件。

---

## Overview / 概述

This plugin provides specialized prompt generation for **Seedance 2.0**, ByteDance's cutting-edge video AI platform. Unlike traditional multi-scene storyboards, this skill understands Seedance's single-shot architecture and automatically splits complex video ideas into independent shots that can be generated separately and stitched together.

此插件专为字节跳动的**Seedance 2.0**视频AI平台提供提示词生成。不同于传统的多场景分镜，本技能理解Seedance的单镜头架构，自动将复杂视频想法拆分成可独立生成并拼接的镜头组。

## Current Skills / 当前技能

### 🎬 Seedance Shots - 单镜头组生成器

**English:** Specialized prompt generator for Seedance 2.0. Automatically splits your video ideas into 3-4 independent single shots, generates ready-to-use prompts, and provides complete workflow guidance from generation to editing.

**中文:** Seedance 2.0专用提示词生成工具。支持自动拆分创意或保留用户自带分镜，生成可直接使用的单镜头提示词(每镜头≥4秒)，并提供从生成到剪辑的完整工作流指导。

**Key Features / 核心特性:**
- ✨ 智能分镜处理 - 自动拆分或1:1保留用户分镜
- 🎬 交互式问答 - 使用AskUserQuestion工具
- ⏱️ 时长优化 - 所有镜头≥4秒(符合Seedance限制)
- 🇨🇳 中文优先 - 中文输入仅输出中文(避免冗余)
- 📋 完整工作流 - 从构思到剪辑的全流程指导
- 🎨 多模态支持 - 图片、视频、音频素材引用
- 🔧 高级功能 - 视频延长、编辑、角色替换

**Supported Scenarios / 支持场景:**
- 创意变身 (猫变猫娘、魔法特效)
- 产品展示 (360度展示、功能演示)
- 动作场景 (武侠对打、运动镜头)
- 情感叙事 (人物故事、MV片段)
- 视频延长 (延续已有视频)
- 视频编辑 (角色替换、剧情颠覆)

---

## Why Seedance-Focused? / 为什么专注Seedance?

### The Problem with Generic Storyboards / 通用分镜的问题

Traditional multi-scene storyboards include:
- ❌ Timeline control (0-3s, 3-7s)
- ❌ Scene transitions (fade, dissolve)
- ❌ Multi-scene descriptions

These **don't work** with Seedance 2.0 because it's a **single-shot video model**.

传统多场景分镜包含:
- ❌ 时间轴控制(0-3秒、3-7秒)
- ❌ 转场效果(淡入淡出、溶解)
- ❌ 多场景描述

这些在Seedance 2.0上**无法工作**，因为它是**单镜头视频模型**。

### The Seedance 2.0 Solution / Seedance 2.0方案

**Correct Workflow:**
1. User provides video idea
2. AI splits into 3-4 independent single shots
3. Each shot generates one video segment
4. Stitch segments in CapCut (剪映)
5. Export final video

**正确流程:**
1. 用户提供视频想法
2. AI拆分成3-4个独立单镜头
3. 每个镜头生成一段视频
4. 在剪映中拼接片段
5. 导出成片

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

### Trigger Phrases / 触发词

**English:**
- "Create video shots for..."
- "Generate Seedance prompts for..."
- "Help me make a video about..."

**中文:**
- "帮我生成一个...的视频镜头"
- "为...创建Seedance提示词"
- "制作关于...的视频"

### Example Workflow / 工作流示例

```
用户: 黑白奶牛猫从床头柜跳到床上,在空中变身成女仆猫娘

Claude: (使用AskUserQuestion询问时长、风格等)

用户: 选择8-10秒、写实风格、无素材

Claude: 输出以下镜头组

=== Seedance 2.0 镜头组 · 可直接生成 ===
总时长:10s | 4:3 | Seedance 2.0

📍 镜头1(2.5s)
画面:黑白奶牛猫蹲在木质床头柜上,注视床铺准备跳跃,午后柔光,中景侧推,浅景深,写实毛发
关键词:cat, realistic, ready to jump, soft light, push in

📍 镜头2(4s)
画面:猫咪跃向空中,金色光粒子环绕变身猫娘,黑白女仆装逐渐形成,慢动作,镜头缓慢环绕
关键词:transformation, golden particles, cat girl, slow motion

📍 镜头3(2.5s)
画面:猫娘轻盈落在柔软白色床铺上,裙摆飘动,广角镜头轻微上摇,温馨自然光
关键词:landing, maid outfit, soft bed, wide shot

📍 镜头4(1s)
画面:猫娘面部特写,猫耳灵动,俏皮微笑,柔和面光,浅景深
关键词:close-up, cat ears, playful, realistic

=== 📋 使用方法 ===
1. 在Seedance 2.0中,每个镜头单独生成视频
2. 将生成的4段视频导入剪映
3. 按镜头顺序拼接,即可得到完整10秒短片

[更多提示和技术限制...]
```

---

## What Gets Generated / 生成内容

### 1. Single-Shot Prompts / 单镜头提示词

Each shot includes:
- 📹 Scene description (画面)
- 🏷️ Keywords (关键词)
- ⏱️ Duration (时长)
- 🎥 Camera movement (镜头运动)

### 2. Usage Instructions / 使用说明

Step-by-step guide for:
- Generating each shot in Seedance
- Stitching in CapCut (剪映)
- Recommended settings

### 3. Pro Tips / 专业建议

- Aspect ratio selection
- Generation mode recommendations (Standard vs Creative)
- Multi-modal reference usage

---

## Documentation / 文档

### Core Documents / 核心文档

- **[SKILL.md](skills/seedance-shots/SKILL.md)** - Main skill logic
- **[Quick Reference](skills/seedance-shots/references/quick-reference.md)** - Fast lookup guide
- **[Technical Specs](skills/seedance-shots/references/technical-specs.md)** - Seedance 2.0 limitations
- **[Workflow Guide](skills/seedance-shots/references/workflow-guide.md)** - Complete workflow

### Examples / 示例

**基础场景(来自豆包精选):**
- **[写实治愈-午后窗边猫咪](skills/seedance-shots/examples/realistic-cat-sunlight.md)** - 宠物短视频、治愈系内容
- **[日系二次元-樱花少女](skills/seedance-shots/examples/anime-sakura-girl.md)** - 动漫风格、唯美治愈
- **[电影感夜景-城市街拍](skills/seedance-shots/examples/cinematic-night-street.md)** - 都市Vlog、情绪片段
- **[古风仙侠-飘逸女子](skills/seedance-shots/examples/ancient-chinese-fairy.md)** - 古装短视频、国风内容
- **[赛博朋克-雨夜都市](skills/seedance-shots/examples/cyberpunk-rainy-city.md)** - 科幻短视频、未来场景
- **[海边日落-逆光人像](skills/seedance-shots/examples/sunset-beach-silhouette.md)** - 治愈系、旅行Vlog
- **[3D卡通-草地萌宠](skills/seedance-shots/examples/3d-cartoon-puppy.md)** - 儿童内容、萌宠视频
- **[高级静物-咖啡展示](skills/seedance-shots/examples/coffee-product-display.md)** - 产品广告、美食短视频
- **[情绪光影-室内人像](skills/seedance-shots/examples/moody-indoor-portrait.md)** - 情感短片、艺术人像

### Templates / 模板

- **[Single Shot Template](skills/seedance-shots/templates/single-shot-template.md)** - Prompt templates
- **[Output Format](skills/seedance-shots/templates/output-format.md)** - Standard format specs

---

## Key Improvements / 核心改进

### Before (Generic Storyboard) / 之前(通用分镜)

```
场景1(5秒):远景推近,海边夕阳,女孩跳舞...
场景2(4秒):中景环绕,旋转起舞...
场景3(7秒):近景特写,表情特写...
```
→ Seedance无法理解,会崩坏

### After (Seedance Shots) / 之后(Seedance镜头组)

```
镜头1(2.5s):猫蹲在床头柜准备跳跃
镜头2(4s):猫跃向空中,光粒子环绕变身
镜头3(2.5s):猫娘落在床上
镜头4(1s):猫娘特写表情
```
→ 每个镜头单独生成,剪映拼接

---

## Seedance 2.0 Technical Specs / 技术规格

| Parameter / 参数 | Limit / 限制 |
|------------------|--------------|
| **Duration per shot / 单段时长** | **4-15秒(最低4秒)** |
| Aspect ratio / 比例 | 16:9, 9:16, 1:1, 4:3 |
| Image inputs / 图片素材 | ≤9张, <30MB/张 |
| Video inputs / 视频素材 | ≤3个, 2-15秒, <50MB |
| Audio inputs / 音频素材 | ≤3个, ≤15秒, <15MB |
| Total files / 总文件数 | ≤12个 |
| **Prohibited / 禁止** | 写实真人脸部素材 |
| **Note / 注意** | 所有镜头≥4s,可在剪映调速 |

---

## Language Strategy / 语言策略

**Smart Language Matching:**
- 中文输入 → 仅中文输出 (无英文冗余)
- English input → English output only
- No bilingual redundancy (unless requested)

**Why?**
- Seedance 2.0 is a ByteDance product (Chinese users primary)
- Dual-language output creates clutter
- Users can request language switch anytime

---

## Advanced Features / 高级功能

### 1. Multi-Modal References / 多模态引用

```
📍 镜头1(3s)
画面:参考@图片1的角色形象,在@图片2的场景中...
素材:@图片1(角色)、@图片2(场景)
```

### 2. Video Extension / 视频延长

```
=== Seedance 2.0 延长镜头组 ===
基于视频:@视频1(原视频)
延长时长:5s

📍 延长镜头1(2.5s)
画面:延续@视频1的风格,[新内容]...
```

### 3. Video Editing / 视频编辑

```
=== Seedance 2.0 编辑镜头 ===
原视频:@视频1

📍 编辑镜头1(原视频时长)
保留:@视频1的运镜
修改:将角色换成@图片1的形象
```

---

## Common Scenarios / 常见场景

### Transformation Effects / 变身特效
- Cat to cat-girl / 猫变猫娘
- Magic transformations / 魔法变身
- Character evolution / 角色进化

### Product Showcase / 产品展示
- 360° product views / 360度展示
- Feature highlights / 功能亮点
- Commercial ads / 商业广告

### Action Sequences / 动作场景
- Fighting scenes / 打斗场景
- Sports movements / 运动镜头
- Dance routines / 舞蹈动作

### Emotional Narratives / 情感叙事
- Character stories / 人物故事
- MV clips / MV片段
- Atmospheric scenes / 氛围场景

---

## Tips for Best Results / 最佳效果技巧

### 中文建议
1. **明确想法** - 一句话概括视频内容
2. **合理时长** - 8-10秒是最佳长度
3. **简化动作** - 每个镜头只做一件事
4. **柔和过渡** - 变身用"光粒子"而非"突然"
5. **多次生成** - 重要镜头生成多次选最佳

### English Tips
1. **Clear concept** - One-sentence video description
2. **Optimal duration** - 8-10 seconds works best
3. **Simplified actions** - One action per shot
4. **Smooth transitions** - Use "light particles" not "suddenly"
5. **Multiple attempts** - Generate key shots multiple times

---

## Future Skills / 未来技能

Within prompt-gen plugin:
- 📸 **Seedance Image** - Image-to-video prompts
- 🎵 **Music Sync** - Beat-matching video prompts
- 🎬 **Long-form Narrative** - 30s+ complex stories

---

## Migration from Storyboard / 从Storyboard迁移

If you previously used `prompt-gen:storyboard`:
- Skill has been renamed to `prompt-gen:seedance-shots`
- Logic completely rewritten for single-shot architecture
- Old prompts **will not work** with Seedance 2.0
- Please use the new skill for better results

如果您之前使用`prompt-gen:storyboard`:
- 技能已重命名为`prompt-gen:seedance-shots`
- 逻辑完全重写为单镜头架构
- 旧提示词在Seedance 2.0上**无法工作**
- 请使用新技能以获得更好效果

---

## Contributing / 贡献

This is a personal skill library, but suggestions and improvements are welcome!

这是个人技能库，但欢迎提出建议和改进！

Open an issue for:
- Bug reports / 错误报告
- Feature requests / 功能请求
- Example contributions / 示例贡献

---

## Version History / 版本历史

**v1.0.0** (2024-02-13)
- Complete refactor from generic storyboard to Seedance-specific
- Renamed skill: storyboard → seedance-shots
- Implemented single-shot splitting logic
- Added interactive AskUserQuestion workflow
- Chinese-first language strategy
- Added 10+ comprehensive examples
- Created quick reference and technical specs
- Added multi-modal reference support
- Added video extension and editing features

**v0.1.0** (2024-02-12)
- Initial release (generic storyboard)
- Deprecated due to platform mismatch

---

## License / 许可证

MIT License - See root LICENSE file

---

## Author / 作者

**DR1N0**

Specialized skills for professional AI video creation workflows.

专为专业AI视频创作工作流设计的技能。

---

## Resources / 相关资源

- **Seedance 2.0:** https://jimeng.jianying.com
- **CapCut (剪映):** https://www.capcut.cn
- **Claude Code Plugins:** https://docs.anthropic.com/claude/docs/plugins

---

## Feedback / 反馈

Questions or feedback? / 问题或反馈？

Create an issue in the repository or reach out via GitHub.

在仓库中创建issue或通过GitHub联系。
