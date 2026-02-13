---
name: storyboard
description: This skill should be used when the user asks to "create a storyboard", "generate video scenes", "storyboard a video", "plan video shots", "创建分镜", "生成视频场景", "分镜脚本", "视频分镜", or mentions video AI generation tools like Seedance, Runway, or similar platforms
version: 0.1.0
---

# Interactive Storyboard Workflow for Video AI Generation

## Purpose

Guide users through creating detailed, production-ready storyboards optimized for video AI generation tools (Seedance 2.0, Runway, Pika, etc.). This interactive workflow collects all necessary information scene-by-scene and outputs structured prompts.

## Language Detection

**Detect user's language from their initial request and respond accordingly throughout the workflow.**

- If user writes in Chinese (中文), respond in Chinese
- If user writes in English, respond in English
- Maintain consistency throughout the interaction

## Workflow Steps

### Step 1: Project Overview

Collect basic project information:

**English prompts:**
- What is the video title/theme?
- What is the target duration? (e.g., 15s, 30s, 1min, 5min)
- What is the overall mood/style? (e.g., cinematic, playful, dramatic, minimalist)
- What is the intended use? (commercial, social media, short film, tutorial, etc.)

**中文提示:**
- 视频标题/主题是什么？
- 目标时长？(例如：15秒、30秒、1分钟、5分钟)
- 整体情绪/风格？(例如：电影感、活泼、戏剧性、极简主义)
- 用途？(广告、社交媒体、短片、教程等)

### Step 2: Scene Planning

Ask how many scenes the storyboard should have. Recommend:
- 15-30s video: 3-5 scenes
- 30-60s video: 5-8 scenes
- 1-3min video: 8-15 scenes
- Longer content: 15+ scenes

### Step 3: Scene-by-Scene Collection

For EACH scene, collect the following information interactively:

**Scene Number & Duration**
- Scene index (1, 2, 3...)
- Duration in seconds

**Visual Description**
- Main subject/action (what's happening)
- Setting/environment (where)
- Characters/objects present
- Visual style elements (colors, lighting, composition)

**Camera & Movement**
- Camera angle (wide shot, medium shot, close-up, extreme close-up, POV, aerial, etc.)
- Camera movement (static, pan left/right, tilt up/down, zoom in/out, dolly, tracking, orbit, etc.)
- Lens type if specific (wide angle, telephoto, fish-eye)

**Mood & Atmosphere**
- Emotional tone (joyful, tense, peaceful, energetic, mysterious, etc.)
- Lighting (bright, moody, golden hour, dramatic shadows, soft, harsh, etc.)
- Color palette (warm, cool, vibrant, muted, monochrome, etc.)

**Transition**
- How to transition to next scene (cut, fade, dissolve, wipe, zoom, match cut, etc.)

**Additional Notes**
- Any specific requirements or references
- Text overlays or graphics needed

### Step 4: Generate Optimized Prompts

After collecting all scene information, generate two outputs:

#### Output 1: Storyboard Table

Create a markdown table with all scenes:

```markdown
| Scene | Duration | Visual Description | Camera | Mood | Transition |
|-------|----------|-------------------|---------|------|------------|
| 1     | 3s       | ...               | ...     | ...  | ...        |
```

#### Output 2: AI-Ready Prompts

For each scene, generate an optimized prompt formatted for video AI tools:

**Prompt structure:**
```
Scene [N]: [Duration]s

[Detailed visual description], [camera angle and movement], [lighting and mood], [style notes]

Keywords: [comma-separated relevant terms]
```

**Example:**
```
Scene 1: 3s

A bustling Tokyo street at night, neon signs reflecting on wet pavement, people with umbrellas walking past. Wide establishing shot, slow dolly forward. Cinematic cyberpunk aesthetic with vibrant pink and blue neon lights casting dramatic shadows. Rain creates atmosphere and depth.

Keywords: Tokyo, night, neon, rain, cyberpunk, wide shot, cinematic, urban
```

### Step 5: Review & Refinement

Present the complete storyboard and ask:
- Does anything need adjustment?
- Should any scenes be split or combined?
- Are all prompts optimized for AI generation?

Iterate based on feedback.

### Step 6: Export Options

Offer to export in different formats:
- Markdown table (for documentation)
- Plain text prompts (for copy-paste to AI tools)
- Numbered list with full details
- JSON format (for programmatic use)

## Best Practices for Video AI Prompts

### Be Specific
- Include concrete details about subjects, actions, environment
- Specify camera angles and movements clearly
- Describe lighting and mood explicitly

### Use AI-Friendly Language
- Start with the main subject/action
- Use descriptive adjectives and adverbs
- Include style references when relevant (e.g., "Wes Anderson style", "documentary footage", "anime aesthetic")

### Optimize for Coherence
- Maintain consistent subjects across scenes for continuity
- Use similar style descriptors throughout
- Plan transitions that AI can execute smoothly

### Include Technical Details
- Camera specifications (wide angle, telephoto)
- Lighting conditions (golden hour, studio lighting, natural light)
- Movement dynamics (slow motion, time-lapse, normal speed)

## Example Interaction Flow

**User:** "Create a storyboard for a 30-second coffee commercial"

**Assistant:**
Great! Let's create a storyboard for your coffee commercial.

**Project Details:**
- Duration: 30 seconds
- Purpose: Commercial

Let me ask a few questions:
1. What's the overall mood? (e.g., cozy morning, energetic, luxury, artisanal)
2. What's the key message or selling point?
3. Any specific settings? (café, home kitchen, nature, urban)

[Continue interactive dialogue...]

## Bilingual Support Notes

When user speaks Chinese:
- Use Chinese for all questions and explanations
- Keep the same workflow structure
- Generate bilingual output if requested
- Use Chinese terminology for camera angles and techniques

## References

For more detailed guidance:
- See `references/workflow-guide.md` for comprehensive documentation
- See `examples/` directory for complete storyboard samples
- Camera terminology: wide shot (远景), close-up (特写), pan (横摇), tilt (竖摇)

## Output Quality Standards

Ensure all generated prompts:
✓ Are specific and detailed (not vague)
✓ Include camera and movement information
✓ Specify lighting and mood
✓ Use AI-friendly descriptive language
✓ Maintain consistency across scenes
✓ Are optimized for the specified duration
✓ Include relevant keywords
✓ Are ready to copy-paste into video AI tools

## Common Video Types & Recommendations

**Commercial (15-30s):**
- 3-5 impactful scenes
- Focus on product features and emotional connection
- Strong opening and call-to-action ending

**Social Media (15-60s):**
- Hook in first 2 seconds
- Fast-paced scene changes
- Vertical format considerations

**Short Film (1-5min):**
- Story arc with setup, conflict, resolution
- More scenes for narrative development
- Varied camera angles for visual interest

**Tutorial/Educational (2-10min):**
- Clear step-by-step progression
- Medium shots and close-ups for clarity
- Consistent style for professionalism

---

**Remember:** This is an interactive, iterative process. Ask clarifying questions, show examples, and refine based on user feedback to create the perfect storyboard for their video AI generation needs.
