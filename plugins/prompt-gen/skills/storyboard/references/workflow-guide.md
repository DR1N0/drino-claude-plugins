# Storyboard Workflow Guide / 分镜工作流指南

## Overview / 概述

**English:** This guide provides comprehensive documentation for creating professional storyboards optimized for video AI generation tools like Seedance 2.0, Runway ML, Pika, and other text-to-video platforms.

**中文:** 本指南为创建专业分镜脚本提供全面文档，针对Seedance 2.0、Runway ML、Pika等视频AI生成工具进行优化。

---

## Camera Terminology / 摄影术语

### Camera Angles / 机位角度

| English | 中文 | Description / 描述 |
|---------|------|-------------------|
| Wide Shot (WS) | 远景 | Shows full subject and surroundings / 显示完整主体和周围环境 |
| Medium Shot (MS) | 中景 | Shows subject from waist up / 显示主体腰部以上 |
| Close-Up (CU) | 特写 | Shows face or object details / 显示面部或物体细节 |
| Extreme Close-Up (ECU) | 大特写 | Very tight on specific detail / 非常紧密的特定细节 |
| Over-the-Shoulder (OTS) | 过肩镜头 | View from behind one subject / 从一个主体背后观看 |
| Point of View (POV) | 主观镜头 | Camera as character's eyes / 摄像机作为角色的眼睛 |
| Bird's Eye View | 鸟瞰 | Looking straight down / 垂直向下看 |
| Aerial Shot | 航拍 | High angle from above / 从上方的高角度 |
| Low Angle | 低角度 | Camera below subject looking up / 摄像机在主体下方向上看 |
| High Angle | 高角度 | Camera above subject looking down / 摄像机在主体上方向下看 |
| Dutch Angle | 荷兰角 | Tilted horizon line / 倾斜的地平线 |

### Camera Movements / 镜头运动

| English | 中文 | Description / 描述 |
|---------|------|-------------------|
| Static | 静止 | No camera movement / 无摄像机移动 |
| Pan | 横摇 | Rotate left/right on axis / 在轴上左右旋转 |
| Tilt | 竖摇 | Rotate up/down on axis / 在轴上上下旋转 |
| Dolly/Track | 移动车 | Camera moves toward/away / 摄像机向前/向后移动 |
| Zoom | 变焦 | Lens zooms in/out / 镜头变焦 |
| Crane/Boom | 升降 | Camera moves up/down / 摄像机上下移动 |
| Orbit | 环绕 | Camera circles around subject / 摄像机围绕主体旋转 |
| Handheld | 手持 | Shaky, dynamic movement / 晃动、动态的移动 |
| Steadicam | 稳定器 | Smooth tracking movement / 平滑的跟踪移动 |

---

## Lighting Terminology / 灯光术语

### Lighting Conditions / 光照条件

| English | 中文 | When to Use / 使用场景 |
|---------|------|----------------------|
| Golden Hour | 黄金时刻 | Warm, soft outdoor light / 温暖柔和的户外光线 |
| Blue Hour | 蓝调时刻 | Cool twilight ambiance / 凉爽的黄昏氛围 |
| Harsh Light | 硬光 | Strong shadows, high contrast / 强烈阴影，高对比度 |
| Soft Light | 柔光 | Diffused, minimal shadows / 漫射，最小阴影 |
| Backlight | 背光 | Light from behind subject / 从主体后方照明 |
| Rim Light | 轮廓光 | Highlights subject edges / 突出主体边缘 |
| Natural Light | 自然光 | Daylight, no artificial sources / 日光，无人工光源 |
| Studio Lighting | 棚灯 | Controlled artificial setup / 可控的人工设置 |
| Neon Lighting | 霓虹灯 | Colorful artificial glow / 彩色人工光芒 |
| Candlelight | 烛光 | Warm, flickering, intimate / 温暖、闪烁、私密 |

---

## Mood & Atmosphere / 情绪与氛围

### Emotional Tones / 情感基调

**Positive / 正面:**
- Joyful / 欢乐的
- Peaceful / 平和的
- Energetic / 充满活力的
- Inspiring / 鼓舞人心的
- Playful / 俏皮的
- Romantic / 浪漫的

**Neutral / 中性:**
- Calm / 平静的
- Contemplative / 沉思的
- Mysterious / 神秘的
- Surreal / 超现实的

**Negative / 负面:**
- Tense / 紧张的
- Melancholic / 忧郁的
- Dramatic / 戏剧性的
- Ominous / 不祥的
- Chaotic / 混乱的

---

## Color Palettes / 色彩方案

### Common Palettes / 常见配色

| Palette | Description EN | 描述 ZH | Use Cases |
|---------|---------------|---------|-----------|
| Warm | Red, orange, yellow tones | 红、橙、黄色调 | Cozy, energetic, sunset scenes |
| Cool | Blue, green, purple tones | 蓝、绿、紫色调 | Technology, night, calm scenes |
| Monochrome | Single color variations | 单色变化 | Artistic, minimalist, retro |
| Vibrant | High saturation colors | 高饱和度颜色 | Playful, youthful, energetic |
| Muted | Desaturated, pastel | 降低饱和度、柔和 | Elegant, vintage, sophisticated |
| Complementary | Opposite color wheel | 互补色 | High contrast, dynamic |
| Analogous | Adjacent colors | 相邻色 | Harmonious, natural |

---

## Video AI Prompt Engineering / 视频AI提示词工程

### Prompt Structure Formula / 提示词结构公式

```
[Subject] + [Action] + [Setting] + [Camera] + [Lighting] + [Mood] + [Style]
```

**Example:**
```
A young woman drinking coffee + sitting by window + cozy café interior + medium shot, dolly in slowly + soft morning light streaming through window + peaceful, contemplative + cinematic, warm tones
```

### Best Practices / 最佳实践

**English:**

1. **Start with the main subject** - What is the focus?
2. **Describe the action** - What is happening?
3. **Set the scene** - Where does this take place?
4. **Specify camera work** - How should it be framed and move?
5. **Define lighting** - What's the light quality?
6. **Convey mood** - What should viewers feel?
7. **Add style notes** - Any specific aesthetic?

**中文:**

1. **从主要主体开始** - 焦点是什么？
2. **描述动作** - 正在发生什么？
3. **设置场景** - 这发生在哪里？
4. **指定摄影机工作** - 应该如何构图和移动？
5. **定义照明** - 光线质量如何？
6. **传达情绪** - 观众应该感受到什么？
7. **添加风格注释** - 任何特定的美学？

### Common Pitfalls to Avoid / 避免常见错误

❌ **Too vague:** "A nice scene"
✓ **Specific:** "A sunlit forest clearing with rays of light through trees"

❌ **Too complex:** "A person walking while thinking about their childhood memories while birds fly overhead and..."
✓ **Focused:** "A person walking slowly through a park, looking contemplative"

❌ **Missing camera info:** "A car driving"
✓ **Complete:** "A red sports car driving on coastal highway, tracking shot from side, golden hour"

---

## Transition Types / 转场类型

### Visual Transitions / 视觉转场

| Type | 中文 | Description | Best For |
|------|------|-------------|----------|
| Cut | 切 | Instant change | Fast-paced, energetic |
| Fade to Black | 淡入黑 | Gradual to black | End of scene, dramatic pause |
| Dissolve | 叠化 | Blend two scenes | Passage of time, dreamlike |
| Wipe | 划像 | One scene pushes other | Retro, stylized |
| Zoom Transition | 缩放转场 | Zoom into/out of detail | Modern, dynamic |
| Match Cut | 匹配剪辑 | Similar shapes/actions | Clever, artistic |
| Whip Pan | 快速摇镜 | Very fast pan | Energetic, surprising |

---

## Scene Duration Guidelines / 场景时长指南

### Optimal Scene Lengths / 最佳场景长度

**For Different Video Types:**

**Commercial / 广告 (15-30s total):**
- Opening: 2-4s (grab attention)
- Middle: 1-3s per scene (2-3 scenes)
- Closing: 3-5s (call-to-action)

**Social Media / 社交媒体 (15-60s):**
- Hook: 1-2s (must grab immediately)
- Content: 2-4s per scene
- Ending: 2-3s

**Cinematic / 电影感 (60s+):**
- Establishing: 4-8s
- Action: 3-6s per scene
- Emotional beats: 5-10s

**Tutorial / 教程:**
- Introduction: 5-10s
- Each step: 10-20s
- Conclusion: 5-10s

---

## Platform-Specific Considerations / 平台特定考虑

### Seedance 2.0 Optimization / Seedance 2.0优化

**Strengths / 优势:**
- Handles complex camera movements well
- Good with realistic lighting
- Excels at outdoor scenes

**Prompt Tips:**
- Be specific about movement speed
- Include weather conditions for outdoor
- Specify realistic vs stylized

### Runway ML

**Strengths:**
- Great for abstract and artistic
- Smooth motion interpolation
- Good text-to-video capabilities

**Prompt Tips:**
- Emphasize style keywords
- Describe motion dynamics clearly
- Reference art styles when relevant

### Pika

**Strengths:**
- Fast generation
- Good for quick iterations
- Handles modifications well

**Prompt Tips:**
- Clear, concise prompts work best
- Specify frame rate when needed
- Use simple camera movements

---

## Advanced Techniques / 高级技巧

### Continuity Planning / 连续性规划

**English:** Ensure visual continuity across scenes:
- Maintain consistent lighting direction
- Keep character appearance stable
- Use similar color grading throughout
- Plan for smooth transitions

**中文:** 确保场景之间的视觉连续性：
- 保持一致的光线方向
- 保持角色外观稳定
- 在整个过程中使用相似的色彩分级
- 规划平滑的过渡

### Keywords Strategy / 关键词策略

**High-Impact Keywords:**
- Cinematic
- 4K
- Professional
- Dramatic
- Atmospheric
- Dynamic
- Photorealistic

**Style References:**
- "Wes Anderson style" - symmetrical, pastel colors
- "Christopher Nolan style" - epic, dramatic
- "Documentary footage" - realistic, raw
- "Music video aesthetic" - stylized, creative

---

## Example Storyboards / 示例分镜

### 30-Second Coffee Commercial / 30秒咖啡广告

**Scene 1 (5s):**
- **Visual:** Close-up of coffee beans being poured into grinder
- **Camera:** Extreme close-up, slow motion
- **Lighting:** Warm morning light
- **Mood:** Anticipation, sensory
- **Transition:** Match cut to grinding

**Scene 2 (4s):**
- **Visual:** Steam rising from brewing coffee
- **Camera:** Medium shot, slight tilt up following steam
- **Lighting:** Backlit, dramatic
- **Mood:** Aromatic, inviting
- **Transition:** Dissolve

**Scene 3 (6s):**
- **Visual:** Hands wrapping around warm coffee mug
- **Camera:** Close-up, static
- **Lighting:** Soft, cozy indoor light
- **Mood:** Comfort, warmth
- **Transition:** Cut

**Scene 4 (8s):**
- **Visual:** Person enjoying coffee while looking out window at sunrise
- **Camera:** Medium shot, dolly in slowly
- **Lighting:** Golden hour through window
- **Mood:** Peaceful, satisfied
- **Transition:** Fade to black

**Scene 5 (7s):**
- **Visual:** Product shot with tagline
- **Camera:** Static, centered
- **Lighting:** Studio lighting, clean
- **Mood:** Professional, premium
- **Transition:** End

---

## Troubleshooting / 故障排除

### Common Issues / 常见问题

**Problem:** AI generates inconsistent visuals across scenes
**Solution:** Use very specific character/object descriptions, maintain same keywords

**Problem:** Camera movements too subtle or exaggerated
**Solution:** Add qualifiers like "slowly", "gradually", "dramatically"

**Problem:** Wrong mood or atmosphere
**Solution:** Add multiple mood descriptors, reference specific lighting conditions

**Problem:** Transitions don't work smoothly
**Solution:** Ensure visual elements in adjacent scenes have some connection

---

## Resources / 资源

### Further Reading / 延伸阅读

- Cinematography basics
- Color theory for video
- Shot composition rules
- Video editing fundamentals

### Tools / 工具

- Seedance 2.0: https://seed.bytedance.com
- Runway ML: Video AI platform
- Pika: AI video generation
- Midjourney: Reference for visual styles

---

**Remember:** Great storyboards balance specificity with creative flexibility. Provide enough detail for AI to generate quality visuals while leaving room for interesting interpretations.

好的分镜脚本在具体性和创造性灵活性之间取得平衡。提供足够的细节让AI生成高质量的视觉效果，同时为有趣的诠释留出空间。
