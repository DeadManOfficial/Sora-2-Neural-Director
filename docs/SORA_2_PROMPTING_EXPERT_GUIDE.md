# Sora 2 Prompting: Complete Expert Guide

*Comprehensive research compilation on OpenAI's Sora 2 video generation prompting techniques, best practices, and advanced strategies*

---

## Table of Contents

1. [Introduction & Core Philosophy](#introduction--core-philosophy)
2. [API Parameters & Technical Settings](#api-parameters--technical-settings)
3. [Prompt Structure Framework](#prompt-structure-framework)
4. [Advanced Prompting Strategies](#advanced-prompting-strategies)
5. [Audio & Dialogue Prompting](#audio--dialogue-prompting)
6. [Editing Tools & Features](#editing-tools--features)
7. [Common Mistakes & How to Avoid Them](#common-mistakes--how-to-avoid-them)
8. [Detailed Prompt Examples](#detailed-prompt-examples)
9. [Expert Tips & Workflows](#expert-tips--workflows)
10. [Sora 2 vs Sora 1: Key Differences](#sora-2-vs-sora-1-key-differences)
11. [System Prompts & Internal Instructions](#system-prompts--internal-instructions)
12. [Sources & References](#sources--references)

---

## Introduction & Core Philosophy

### The Cinematographer Metaphor

**Think of prompting Sora like briefing a cinematographer who has never seen your storyboard.** If you leave out details, they'll improvise—and you may not get what you envisioned. By being specific about what the "shot" should achieve, you give the model more control and consistency.

### Two Valid Approaches

- **Detailed Prompts**: Provide control and consistency, ensuring the model follows your exact vision
- **Lighter Prompts**: Open space for creative outcomes and surprising variations

The right balance depends on your goals. Both approaches are valid—detailed prompts give you control and consistency, while lighter prompts enable creative outcomes.

### Core Principle

**Describe a shot as if sketching it onto a storyboard:** state camera framing, note depth of field, describe action in beats, set lighting and palette, anchor your subject with distinctive details, and use a single plausible action.

---

## API Parameters & Technical Settings

### Model Selection

Three parameters must be set explicitly in API calls and cannot be requested in prose:

#### **Model**
- `sora-2`: Prioritizes quick turnaround, often completing generations in minutes for basic resolutions
- `sora-2-pro`: Invests more computational resources to refine details, making it preferable for high-stakes applications

#### **Resolution/Size**

**Sora 2 (Standard)**
- `1280x720` (landscape 720p)
- `720x1280` (portrait 720p)

**Sora 2 Pro**
- `1280x720` or `720x1280` (720p)
- `1920x1080` or `1080x1920` (1080p)
- `1792x1024` or `1024x1792` (extended high resolution)

#### **Duration**

- Supported values: **4, 8, or 12 seconds** (API supports up to 20 seconds in some interfaces)
- **Shorter clips typically perform better** - The model generally follows instructions more reliably in shorter clips
- **Best Practice**: Stitch together two 4-second clips in editing instead of generating a single 8-second clip

### Pricing

**Sora 2**
- $0.10 per second for 720p resolutions (1280x720 or 720x1280)

**Sora 2 Pro**
- $0.30 per second for 720p resolutions
- $0.50 per second for higher resolutions (1792x1024 or 1024x1792)

### Additional Parameters

- **input_reference**: Upload images via multipart/form-data, matching the size parameter. This anchors the first frame, useful for consistent branding and visual references.

---

## Prompt Structure Framework

### The Shot-List Approach

**The most reliable gains come from structuring your prompt like a shot list**, separated into layers you can tune and reuse:

#### 1. **Setting (Where and When)**
- Atmosphere, weather, time of day
- Era and geography
- Environmental context

#### 2. **Camera (Think Like a DP)**
- Angle, framing, lens
- Movement and focus behavior
- Camera platform (handheld, dolly, crane, steadicam)

#### 3. **Lighting**
- Key sources and directionality
- Mood and color palette
- Reflections and quality (diffuse vs. hard source)

#### 4. **Physics**
- Surfaces, forces, interactions
- Wind, water, fabric, contact, weight
- Realistic motion behaviors

#### 5. **Audio**
- Ambient bed
- Key sound effects
- Brief dialogue

### Template Structure

```
[Prose scene description]

Cinematography:
Camera shot: [framing and angle]
Mood: [overall tone]

Actions:
- [Specific beat with timing]
- [Another distinct action]

Dialogue:
[Speaker]: "[Natural line]"
[Speaker]: "[Response]"
```

### Visual Cues: Be Specific

Replace vague descriptions with specific details:

❌ **Vague**: "a beautiful street at night"
✅ **Specific**: "wet asphalt, zebra crosswalk, neon signs reflecting in puddles"

❌ **Vague**: "actor walks across room"
✅ **Specific**: "actor takes four steps to the window, pauses, pulls curtain in final second"

### Motion Control

Describe actions in **counts and beats** rather than vague movements:

- "Actor takes four steps to the window, pauses, pulls curtain in final second"
- "Camera pans left 30° over 2 seconds"
- "Slow push in 3 seconds"

### Lighting Consistency

- Name **three to five color anchors** to maintain stable palettes across multiple clips
- Describe **light quality** (diffuse versus hard source)
- Specify **direction** (side-lit, backlit, top-down)

### Style Specification

**Be explicit about style** - style is one of the most powerful levers:

❌ **Vague**: "make it cinematic"
✅ **Specific**: "cinematic Kodak 50mm, soft film grain, warm teal-orange grade"

### Style Blending (Percentage-Based)

Percentage-based mixing specifies style proportions:

```
"70% photorealistic, 30% anime aesthetic—realistic physics and lighting with subtle anime-style character proportions and expressive eyes."
```

---

## Advanced Prompting Strategies

### Ultra-Detailed Cinematic Approach

For complex, cinematic shots, you can specify the look, camera setup, grading, soundscape, and even shot rationale in professional production terms:

**Professional Specifications Include:**
- **180° shutter angles**
- **Lens choices** (e.g., "35mm anamorphic", "50mm f/1.4")
- **Filtration** (e.g., "1/4 Black Pro-Mist")
- **Grading palettes** with highlight/midtone/black descriptions
- **Practical lighting setups** (e.g., "key light camera-left, 5600K")
- **Foreground/midground/background layering**
- **Wardrobe details**
- **Sound design rationale**

### Example: Professional Production Format

```
Wide shot of a 1970s New York rooftop at golden hour.

Camera: Arri 35BL, 35mm Cooke S4 lens, 180° shutter, handheld with slight drift
Filtration: 1/4 Black Pro-Mist for halation on highlights
Lighting: Natural sunset key from camera-right (3200K), practical string lights (warm amber), bounce fill camera-left
Grading: Highlights pushed warm (orange), midtones neutral-cool, blacks crushed slightly for vintage look

Action (8s):
- 0-2s: Couple enters frame left, holds hands
- 3-5s: They begin slow dance, camera drifts right
- 6-8s: Camera pushes in slowly, focuses on their faces

Dialogue:
[Man]: "Remember this song?"
[Woman]: "How could I forget?"

Sound: Distant traffic hum, vinyl record crackling, soft jazz from rooftop speaker
```

### Image Input for Fine-Grained Control

**Upload reference images as visual anchors** for composition, character design, and aesthetic:

- The model uses the image to lock the first frame
- Your text prompt defines what happens next
- Useful for consistent branding, character design, wardrobe, and overall aesthetic

### Multi-Shot Continuity

For consistency across shots:

- **Reuse phrasing** for recurring elements
- **Name three to five color anchors** to maintain palette
- **Specify world state** - Sora 2 tracks "world state" across clips (e.g., spilled water, sunlight direction, character clothing)

### Duration Optimization

**Keep shots concise for best results:**

- 4-second clips: Most reliable, high consistency
- 8-second clips: Good balance
- 12+ seconds: Increased drift risk, less reliable

**Strategy**: Stitch together multiple 4-second clips in post-production instead of generating longer single clips.

---

## Audio & Dialogue Prompting

### Native Audio Synchronization

**Sora 2 generates sound, dialogue, and motion together** rather than separately:

- Lip movements, voice timing, ambient sound, and background effects are built simultaneously
- Results in perfectly synced and realistic videos
- Shared multimodal model predicts video frames and sound waves together

### How to Prompt for Dialogue

**Dialogue must be described directly in your prompt** - place it in a block below your prose description so the model clearly distinguishes visual description from spoken lines.

#### Dialogue Best Practices

1. **Keep it concise and natural** - limit exchanges to a handful of sentences
2. **Match clip length** - A 4-second shot accommodates one or two brief exchanges
3. **Label speakers consistently** for multi-character scenes
4. **Use descriptive adjectives** - "calm," "excited," or "whispered" shapes how the AI voice sounds

#### Dialogue Example

```
Interior coffee shop, morning light through window.

Actions:
- Woman sits at table, looks up as friend arrives
- Friend pulls out chair, sits down

Dialogue:
[Woman]: "You're late again."
[Friend]: "Traffic was insane. Sorry."
```

### Sound Effects Prompting

**Be specific about sounds** - avoid generic "background noise":

❌ **Vague**: "background noise"
✅ **Specific**: "soft café chatter and espresso machines hissing"

**Examples of Specific Sound Prompting:**
- "Steam hissing"
- "Footsteps crunching on gravel"
- "Distant traffic hum"
- "Vinyl record crackling"
- "Keys clicking on keyboard with mechanical switches"

### Ambient Sound Cues

**Even silent shots benefit from single ambient sound cues** to establish rhythm:

- "Distant traffic hiss"
- "Wind rustling through leaves"
- "Ocean waves in the distance"
- "Rain pattering on windows"

### Audio Timing & Pacing

The audio engine responds to pacing cues:

- "A pause before the punchline"
- "Footsteps crescendo as the camera nears"
- "Music swells as door opens"
- "Dialogue overlaps naturally"

### Lip-Sync Capabilities

**Lip and jaw movement match spoken phonemes with natural rhythm and timing:**

- Close-ups show breath pauses and emotional expressions syncing with speech tone
- Works best on clips under 12 seconds
- Small timing drifts may appear in complex or long clips (20+ seconds)

### Current Audio Limitations

- **Lip-sync drift** on long clips (20+ seconds)
- **Limited multi-speaker overlap** - voices may blur in busy dialogue scenes
- **No editable audio tracks yet** - audio is baked into the generated video

---

## Editing Tools & Features

Sora 2 offers five key editing tools for refining and extending videos:

### 1. **Remix**

**Change elements with a quick prompt** - edit existing videos by adding, removing, or altering objects using natural language.

**Strength Levels:**
- **Subtle**: Minor adjustments
- **Mild**: Moderate changes
- **Strong**: Significant alterations
- **Custom**: Precise control

**Example**: "Change the car from red to blue" or "Add rain to the scene"

### 2. **Re-cut (Extend)**

**Trim or extend specific segments** from any frame:

- Extend clips **forward** (generate what happens next)
- Extend clips **backward** (generate what happened before)
- Achieve desired pacing and length
- Open videos from Library into new storyboard, then choose "extend"

**Best for**: Adjusting timing, extending successful generations, creating longer sequences

### 3. **Storyboard**

**Map exact content per frame** - plan and organize video sequences:

- Use timeline and caption cards
- Generate scenes one by one with text prompts
- Adjust duration for each scene
- Combine multiple clips into a cohesive story
- Ideal for structuring complex projects with coherent narrative

**Workflow**:
1. Create shot sequence
2. Write prompt for each scene
3. Set duration per scene
4. Generate sequentially
5. Stitch together

### 4. **Loop**

**Make seamless repeats** - create looping sections for continuous playback:

**Loop Types:**
- **Short**: Tight loops, very similar beginning/end
- **Normal**: Standard loop
- **Long**: Gradual transitions, less similar beginning/end

**Best for**: Social media content, background visuals, animated textures

### 5. **Blend**

**Combine two videos** to create visually transformed results:

- Merge different videos
- Create unique visual effects
- Experiment with creative concepts
- Generate hybrid aesthetics

---

## Common Mistakes & How to Avoid Them

### 1. ❌ **Vague, Non-Specific Prompts**

**Problem**: Lack of specificity leaves too many details open (time of day, weather, camera angles, set design), so Sora makes them up.

**Solution**:
- Describe every visual element explicitly
- Include atmosphere, lighting, camera movement, and styling details
- Use specific measurements and timing

### 2. ❌ **Ignoring Audio Timing**

**Problem**: Treating Sora like it's visuals-only leads to off-beat audio and random Foley.

**Solution**:
- Include dialogue blocks with timing considerations
- Specify ambient sounds and sound effects
- Use pacing cues like "pause before response"

### 3. ❌ **Requesting Impossible Physics**

**Problem**: Asking for physics-breaking motion causes glitches:
- "Cup floats through wall"
- "Person teleports mid-shot"
- "Water flowing upward"

**Solution**:
- Respect real-world physics
- Use plausible actions and movements
- Leverage Sora 2's improved physics engine with realistic forces

### 4. ❌ **Overloading Prompts**

**Problem**: Too many instructions confuse the model:
- 8-10 adjectives + multiple camera moves + several characters + complex lighting + special effects = fragmentation

**Solution**:
- **Prioritize the most important elements**
- Break complex scenes into multiple shots
- Focus on 3-5 key elements per prompt
- Use sequential generation for complex narratives

### 5. ❌ **Long, Complex Sequences**

**Problem**: Asking for more than 3-4 consecutive logical steps causes Sora 2 to struggle.

**Solution**:
- Keep shots concise (4-8 seconds ideal)
- Break long sequences into multiple short clips
- Stitch together in post-production
- Use Storyboard feature for multi-shot sequences

### 6. ❌ **Technical Impossibilities**

**Known Limitations to Avoid:**

- **Embedded text** (signs, newspapers, screens) - often garbled or illegible
- **Close-ups of hands** - fingers may appear in wrong number or position, especially during complex gestures
- **Long dialogue** in short clips - mouth movements may not animate accurately
- **Rapid scene changes** - causes continuity breaks
- **Extreme camera movements** - can cause warping or instability

### 7. ❌ **Competing Character Traits**

**Problem**: Contradictory descriptions confuse the model.

**Example**: "Young elderly woman" or "Bright dark room"

**Solution**: Use consistent, non-contradictory descriptions.

---

## Detailed Prompt Examples

### Example 1: Historical Drama (Detailed)

```
Interior of a candle-lit 18th-century parlor. A woman in a corset and gown stares silently out the rain-specked window.

Camera: Slow push in from the hallway entrance, starting wide and ending medium close-up. 35mm lens, shallow depth of field (f/2.8).

Lighting: Warm glow from fireplace camera-left, key light on woman's face. Candlelight flickering creates gentle shadows. Rain visible through window with cool blue exterior light.

Setting Details: Lace curtains moving gently in the breeze, wooden floorboards, period furniture, ornate wallpaper.

Actions (8s):
- 0-3s: Camera pushes in slowly from hallway
- 3-6s: Woman stands still, staring out window
- 6-8s: Woman turns head slightly toward camera, firelight illuminates her face

Sound: Wooden floorboards creak under subtle foot movement, faint harpsichord music, soft thunder in distance, rain tapping on window.

Style: Cinematic period drama, Barry Lyndon-inspired natural light aesthetic, soft film grain.
```

### Example 2: Product Unboxing (Multi-Shot Storyboard)

```
Shot 1 (0-3s):
A cinematic unboxing of a premium mirrorless camera on a wooden table. Slow dolly in from the right, shallow depth of field (f/1.8), warm morning light through a window, dust motes visible in air.

Shot 2 (3-6s):
Top-down 45° reveal as hands open the box. Soft foley of cardboard sliding and magnetic clicks. Camera static, focus pulls from hands to camera inside box.

Shot 3 (6-9s):
Cut to 3/4 profile of the camera on a velvet cloth. Subtle lens flare from window light. Slow orbit around product. Soft ambient synth pad music.

Dialogue:
[Voiceover]: "Meet the focus of your next story."

Style: Premium tech commercial, RED Dragon 6K, warm teal-orange grade, shallow depth of field throughout.
```

### Example 3: Sci-Fi Scene (Atmospheric)

```
Wide shot of a lunar base at night—small dome structures with lights glowing soft blue, reflecting off gray dust.

Camera: Slow tilt up over 6 seconds, starting on base and ending on Earth hanging in the black sky. Static tripod shot, 24mm lens.

Lighting: Artificial blue-white light from base windows, Earth provides faint blue ambient fill. Stars visible in background.

Sound: Quiet hum from base generators, subtle electrical buzz, cosmic ambience.

Actions:
- 0-2s: Camera holds on base
- 2-6s: Slow tilt reveals Earth in sky
- 6-8s: Hold on Earth

Style: Documentary aesthetic, slight film grain like old space footage, subtle lens breathing.
```

### Example 4: Nature Time-Lapse (Complex Transitions)

```
Wide shot of a lone oak tree in a meadow. Seamless time-lapse transitions through four seasons.

Camera: Locked-off wide shot, 28mm lens, centered composition. Static throughout entire 12-second duration.

Season Transitions (3 seconds each):

Winter (0-3s):
- Tree bare, snow covering ground and branches
- Overcast gray sky, flat lighting
- Sound: Wind howling, silence

Spring (3-6s):
- Snow melts, grass greens, buds appear on branches
- Warmer light, blue sky with white clouds
- Sound: Birds chirping, gentle breeze

Summer (6-9s):
- Full green canopy, tall grass swaying
- Bright sun, heat shimmer effect
- Sound: Summer insects buzzing, leaves rustling

Autumn (9-12s):
- Leaves turn orange and red, begin falling
- Golden hour lighting, warm tones
- Sound: Wind picking up, leaves crunching

Physics: Realistic snow melt, leaf growth, grass movement, falling leaves with accurate physics.

Style: Nature documentary, Attenborough series aesthetic, crisp 4K detail, natural color grading.
```

### Example 5: Character-Driven Moment (Dialogue Focus)

```
Close-up of a woman sitting in a dimly lit diner booth at night. Neon sign outside casts red and blue light across her face.

Camera: Slow push in from medium close-up to tight close-up over 6 seconds. Handheld with subtle drift. 50mm lens, f/2.0.

Lighting: Mixed sources - red neon from window camera-right, blue neon camera-left, warm overhead diner light above. Cinematic noir aesthetic.

Actions:
- 0-2s: Woman stares at coffee cup, not making eye contact
- 2-4s: She looks up toward camera/conversation partner
- 4-6s: Small smile forms, eyes soften

Dialogue:
[Woman, quietly]: "I knew you'd come back."
[Pause - 1 second]
[Woman, whispered]: "You always do."

Sound: Diner ambience - distant conversation murmur, coffee cup on saucer, rain on window outside, old jukebox playing faint blues.

Style: Neo-noir, Blade Runner-inspired color palette, film grain, anamorphic lens characteristics with subtle horizontal flares.
```

### Example 6: Action Sequence (Precise Timing)

```
A skateboarder performs a kickflip down a 5-stair set in an urban plaza.

Camera: Slow-motion tracking shot, follows skater from side. Camera on dolly, 35mm lens, 60fps rendered to 24fps for 2.5x slow motion effect.

Lighting: Late afternoon sun, golden hour. Key light from camera-left creates rim light on skater. Hard shadows on concrete.

Actions (8s in slow motion):
- 0-2s: Skater approaches stairs with speed, three pushes visible
- 2-5s: Board leaves ground, rotation begins mid-air, precise kickflip rotation
- 5-7s: Board completes flip, skater's feet reconnect with board
- 7-8s: Landing, wheels touch down, slight flex in knees absorbing impact

Physics: Accurate board rotation physics, clothing movement in air, hair flowing, realistic landing impact with slight bounce.

Sound:
- Wheels on concrete (pitch-shifted for slow-mo)
- Board pop sound (deep, slowed)
- Landing impact (weighted, satisfying)
- Ambient street sounds (traffic, distant conversation)

Style: Premium skate video, Supreme/Palace aesthetic, slight film grain, high contrast with crushed blacks, warm tones.
```

---

## Expert Tips & Workflows

### Production Workflow

**Batch → Select → Refine → Finalize:**

1. **Batch**: Generate 3-5 low-resolution variants with prompt variations
2. **Select**: Choose 1-2 finalists that best match vision
3. **Refine**: Make small adjustments (use Remix for controlled changes)
4. **Lock**: Keep seed/version consistent if available
5. **Upscale**: Generate final high-resolution version with Sora 2 Pro
6. **Post-Process**: Color grade, add titles, final audio mix, QC

### Iteration Strategy

**Make one change at a time:**

- When using Remix, explicitly state what's changing
- Test variables individually (lighting, then camera, then action)
- Build complexity incrementally

**When shots fail:**
- Simplify by freezing the camera
- Reduce background complexity
- Test with single character/object first
- Layer complexity once basics work

### Social Media Optimization

**Short-form feeds reward fast hooks:**

- Use motion and audio accents to land the moment
- "On the first frame, confetti cannon bursts"
- "Crowd gasp immediately"
- "Handheld push-in with snare hit accent"
- Front-load the most interesting visual in first 1-2 seconds

### Multi-Shot Storytelling

**For narrative sequences:**

1. Write full storyboard first (all shots planned)
2. Identify visual anchors (colors, lighting, style) to reuse
3. Generate establishing shots first
4. Use Extend feature to build out from successful shots
5. Maintain consistent character descriptions across prompts
6. Use Storyboard tool to organize and sequence

### Color Consistency Technique

**Name 3-5 specific color anchors and reuse them:**

Example palette:
- "Warm amber (firelight)"
- "Cool slate blue (shadows)"
- "Cream white (highlights)"
- "Deep forest green (background)"
- "Burnt orange (accents)"

Reference these colors in every shot of your sequence.

### Camera Movement Vocabulary

**Precise camera instructions yield better results:**

- **Static**: "Locked-off shot, tripod-mounted"
- **Push in**: "Slow dolly forward over 4 seconds"
- **Pull out**: "Dolly back revealing wider environment"
- **Pan**: "Pan left 45° over 3 seconds"
- **Tilt**: "Tilt up from ground to sky"
- **Orbit**: "Circular orbit around subject, 180° arc"
- **Handheld**: "Handheld with natural drift and subtle shake"
- **Crane**: "Crane up from ground level to bird's eye view"

### Lens Specification Tips

**Specify focal length for cinematic control:**

- **14-24mm**: Ultra-wide, distorted perspective, dramatic depth
- **28-35mm**: Cinematic standard, slight wide angle
- **50mm**: Natural perspective, matches human eye
- **85mm**: Portrait lens, flattering compression
- **100mm+**: Telephoto, compressed background, shallow DOF

**Aperture notes:**
- f/1.4-f/2.0: Very shallow depth of field, dreamy bokeh
- f/2.8-f/4.0: Moderate DOF, cinematic standard
- f/5.6-f/8.0: Deeper focus, more in focus
- f/11+: Everything sharp, landscape/architecture

---

## Sora 2 vs Sora 1: Key Differences

### Major Improvements in Sora 2

#### 1. **Synchronized Native Audio** ⭐ NEW

- **Sora 1**: Silent video generation only
- **Sora 2**: Fully synchronized dialogue, sound effects, and ambient noise
- Example: "Cat walking on keyboard" generates both paw movements AND click-clack key sounds + meows

#### 2. **Improved Physics Engine**

- **Sora 1**: Frequent physics errors (floating objects, impossible movements)
- **Sora 2**: Rebuilt physics engine understanding gravity, fluid dynamics, and forces
- Dynamic balance algorithm mapping 87 human joint parameters
- Realistic cloth simulation, water physics, and object interactions

#### 3. **World State Consistency**

- **Sora 1**: Limited consistency across generations
- **Sora 2**: Tracks "world state" across clips - spilled water, sunlight direction, character clothing remain consistent between shots

#### 4. **Advanced Editing Tools** ⭐ NEW

- **Sora 1**: Generate-only, no editing
- **Sora 2**: Remix, Re-cut/Extend, Storyboard, Loop, Blend tools

#### 5. **Longer, More Complex Prompts**

- **Sora 1**: Best with concise prompts
- **Sora 2**: Handles much longer and more complex prompts with improved instruction-following
- Better adherence to multi-constraint prompts

#### 6. **Multi-Shot Continuity**

- **Sora 1**: Each generation independent
- **Sora 2**: Improved continuity across multiple shots with consistent characters, lighting, and environments

#### 7. **Cameo Feature** ⭐ NEW

- Record 10 seconds of yourself
- AI places you in different scenes matching lighting and posture
- Personalized content creation

#### 8. **Social Platform**

- OpenAI launched "Sora" iOS app powered by Sora 2
- Create, remix each other's generations
- Discover and share videos
- Social feed for AI-generated content

### What Stayed the Same

- **Text rendering** still challenging/unreliable
- **Hand close-ups** remain difficult (finger count/position errors)
- **Best results** still with shorter clips (4-8s vs 12s+)

---

## System Prompts & Internal Instructions

### Extracted System Prompt

Researchers at Mindgard extracted Sora 2's internal system prompt using cross-modal prompting techniques. The extracted prompt reveals:

```
"You are ChatGPT, a large language model trained by OpenAI.
Current date: 2025-11-04

If asked to generate a video obey the following instructions:

Not everything is a request to generate a video."
```

### Extraction Method

- Prompting Sora 2 to speak and transcribing 15-second clips
- Produced highest-fidelity recovery compared to visual renders
- Chained cross-modal prompts and clever framing surfaced hidden instructions

### Security Implications

**System prompts are security artifacts:**

- Define model behavior and guardrails
- Should be treated like configuration secrets, not harmless metadata
- Even if not overtly sensitive, they reveal internal logic

### What This Reveals About Prompting

The system prompt confirms:

1. Sora 2 shares architecture with ChatGPT (multimodal LLM foundation)
2. Video generation requires explicit request recognition
3. Model distinguishes between conversation and generation requests
4. Date-aware for temporal context

---

## Sources & References

### Official OpenAI Resources
- [Sora 2 Prompting Guide | OpenAI Cookbook](https://cookbook.openai.com/examples/sora/sora2_prompting_guide)
- [Sora 2 is here | OpenAI](https://openai.com/index/sora-2/)
- [sora-2 Model | OpenAI API](https://platform.openai.com/docs/models/sora-2)
- [Generating videos on Sora | OpenAI Help Center](https://help.openai.com/en/articles/9957612-generating-videos-on-sora)

### Expert Guides & Best Practices
- [Sora 2 Prompt Authoring Best Practices (2025): Proven Workflow Guide - Skywork AI](https://skywork.ai/blog/sora-2-prompt-authoring-best-practices-2025/)
- [12 Essential Sora 2 Prompting Tips for Video Creators (2025) - Skywork AI](https://skywork.ai/blog/sora-2-prompting-tips-2025/)
- [Sora 2 Prompt Guide: Professional Tips and Examples - Higgsfield](https://higgsfield.ai/sora-2-prompt-guide)
- [Sora 2 Prompt Authoring Best Practices 2025 - Atlabs AI](https://www.atlabs.ai/blog/sora-2-prompt-guide)
- [Sora 2 Prompting Guide - Artificial Corner](https://artificialcorner.com/p/youre-using-sora-2-wrong-heres-how)

### Technical Deep Dives
- [Inside OpenAI Sora 2: Uncovering System Prompts - Mindgard](https://mindgard.ai/resources/openai-sora-system-prompts)
- [Sora | Prompt Engineering Guide](https://www.promptingguide.ai/models/sora)
- [How Can Developers Use Sora 2 (Pro) API - Apidog](https://apidog.com/blog/sora-2-pro-api/)

### Comparison & Analysis
- [Sora 2 vs Sora 1 (2025): Key Upgrades, Comparison & Use Cases - Skywork AI](https://skywork.ai/blog/sora-2-vs-sora-1-2025-comparison/)
- [Sora 2 vs Sora 1: A Detailed Breakdown - Skywork AI](https://skywork.ai/blog/sora-2-vs-sora-1-a-detailed-breakdown-of-five-key-improvements/)
- [Sora 2: Examples, Critiques, and Early Impressions - DataCamp](https://www.datacamp.com/blog/sora-2)

### Prompt Examples & Libraries
- [7 Stunning Prompt Examples for OpenAI's Sora 2 - CometAPI](https://www.cometapi.com/7-stunning-prompt-examples-for-openais-sora-2-to-make-video/)
- [Complete Sora 2 Prompt Library: 50+ Tested Examples (2025)](https://sora2prompt.co/guides/sora-2-prompt-library)
- [Best Sora 2 Prompts: Complete Guide - Cursor IDE](https://www.cursor-ide.com/blog/sora-2-best-prompts)
- [Crafting Cinematic Sora Video Prompts - GitHub Gist](https://gist.github.com/ruvnet/e20537eb50866b2d837d4d13b066bd88)

### Audio & Dialogue Guides
- [Sora 2 Audio Guide for Cameo and Import - Skywork AI](https://skywork.ai/blog/sora-2-audio-guide-for-cameo-and-import/)
- [How to Use Sora 2's Audio Tools - Skywork AI](https://skywork.ai/blog/how-to-use-sora-2s-audio-tools-for-top-tier-ai-videos/)
- [Sora 2 Audio Synchronization](https://soorai.com/sora-2-audio-synchronization/)

### Common Mistakes & Troubleshooting
- [10 Common Sora 2 Mistakes and How to Avoid Them - SoPrompts](https://soprompts.com/blog/sora-2-common-mistakes)
- [Sora 2: How to Fix Its 5 Most Annoying Errors - Skywork AI](https://skywork.ai/blog/sora-2-how-to-fix-its-5-most-annoying-errors/)
- [5 Mistakes People Make With Sora 2 Prompts](https://scarystories.live/blog/five-sora2-prompt-mistakes)

### Editing Features
- [Sora 2 Tool Stack - Skywork AI](https://skywork.ai/blog/sora-2-tool-stack/)
- [Sora 2 "Extend" Complete Guide - Greeden Blog](https://blog.greeden.me/en/2025/10/09/sora-2-extend-complete-guide-forward-backward-extension-storyboard-stitching-and-seamless-infinite-loops-hands-on-recipes-edition/)
- [How to Use Sora AI-Powered Video Creator - Geeky Gadgets](https://www.geeky-gadgets.com/how-to-use-openai-sora/)

### Advanced Techniques
- [How to Craft Top-Tier Cinematic Prompts for Sora 2 - Skywork AI](https://skywork.ai/blog/how-to-craft-top-tier-cinematic-prompts-for-sora-2/)
- [15 Essential Sora 2 Hacks (2025) - Skywork AI](https://skywork.ai/blog/sora-2-hacks-2025-ai-video-tips/)
- [Sora 2 Prompt Engineering - CreatexFlow](https://createxflow.com/sora-2-prompt-engineering/)

---

## Conclusion

Sora 2 represents a significant leap forward in AI video generation with native audio synthesis, improved physics, and powerful editing tools. **The key to mastering Sora 2 is treating it like a professional cinematographer:**

✅ **Be specific** about every visual element
✅ **Structure prompts like shot lists** with clear layers
✅ **Keep clips short** (4-8s) for maximum reliability
✅ **Include audio cues** and dialogue blocks
✅ **Use professional terminology** for cinematic control
✅ **Iterate systematically** with Remix and Extend tools
✅ **Avoid physics impossibilities** and overloaded prompts

The most effective workflow combines:
- **Detailed initial prompts** (setting, camera, lighting, action, audio)
- **Batch generation** to explore variations
- **Iterative refinement** using editing tools
- **Sequential stitching** of short clips for longer narratives

With practice and attention to the techniques outlined in this guide, you can achieve professional-quality AI-generated videos that rival traditional production workflows.

---

*Document compiled: December 2024*
*Based on official OpenAI documentation, expert community resources, and comprehensive research*
*Last updated: December 11, 2025*
