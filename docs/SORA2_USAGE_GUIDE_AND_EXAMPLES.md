# SORA 2: COMPREHENSIVE USAGE GUIDE
## How to Use the Complete Prompt Library System

**Version**: 1.0
**Classification**: WORKFLOW GUIDE
**Purpose**: Step-by-step instructions for building production prompts
**Audience**: All users from beginner to expert

---

# TABLE OF CONTENTS

1. [Quick Start Workflow](#quick-start-workflow)
2. [Three-Layer System Explained](#three-layer-system-explained)
3. [Step-by-Step Prompt Building](#step-by-step-prompt-building)
4. [20 Complete Examples](#20-complete-examples)
5. [Troubleshooting Common Issues](#troubleshooting-common-issues)
6. [Advanced Techniques](#advanced-techniques)
7. [DEADMAN BROADCAST Integration](#deadman-broadcast-integration)
8. [Optimization Tips](#optimization-tips)

---

# QUICK START WORKFLOW

## The 3-Step Process

**STEP 1: Choose Base Template**
```
Question: "What am I creating?"
Answer determines template category:

- Narrative scene → CINEMATIC templates (CIN-01 to CIN-05)
- Real-world documentation → DOCUMENTARY templates (DOC-01 to DOC-05)
- Product/brand content → COMMERCIAL templates (COM-01 to COM-05)
- Creative/experimental → ARTISTIC templates (ART-01 to ART-05)
- Product showcase → PRODUCT templates (PRD-01 to PRD-03)
- Character focus → CHARACTER templates (CHR-01 to CHR-03)
- Location/space → ENVIRONMENT templates (ENV-01 to ENV-04)
```

**STEP 2: Add Modular Components**
```
Enhance template with specific elements:

- Camera Movement (from Camera Movement Library)
- Lighting Setup (from Lighting Setup Library)
- Motion Descriptors (from Motion Descriptor Library)
- Composition Framework (from Composition Library)
- Atmosphere Elements (from Atmosphere Library)
- Color Palette (from Color Palette Library)
```

**STEP 3: Apply Style Preset (Optional)**
```
Layer overall aesthetic:

- Film Noir → Dark mystery, high contrast, monochrome
- Cyberpunk → Neon colors, urban night, rain
- Naturalistic → Documentary realism, available light
- Vintage/Retro → 1970s/1980s/1990s period aesthetics
- Modern Commercial → Clean polished, brand-focused
- Analog Horror → VHS degradation, institutional dread
- Dreamlike → Soft ethereal, slow-motion feel
- Minimalist → Clean geometric, negative space
- Gritty Realism → Harsh documentary, urban decay
- Fantasy/Magical → Rich colors, volumetric light
```

---

# THREE-LAYER SYSTEM EXPLAINED

## Layer 1: Base Template (Foundation)

**What it provides:**
- Overall shot structure (duration, aspect, complexity)
- Basic camera specifications (lens, aperture, movement type)
- Fundamental lighting approach (setup type)
- Core composition structure (framing, beat timing)
- Subject/environment relationship

**Example:** CIN-02 Dramatic Portrait provides:
- Portrait framing structure
- 85-135mm lens range
- f/1.4-2.8 shallow DOF approach
- Single key lighting mention
- 8-second beat structure

**What it DOESN'T provide (you customize):**
- Specific subject details
- Exact lighting setup
- Precise camera movement
- Color palette specifics
- Style/mood overlay

---

## Layer 2: Modular Components (Customization)

**What they provide:**
- Specific camera movements (dolly speeds, crane paths)
- Exact lighting setups (three-point, Rembrandt, practical-only)
- Motion characteristics (speed, quality, rhythm)
- Composition techniques (rule of thirds, golden ratio, etc.)
- Atmospheric elements (fog, rain, particles)
- Color palettes (earth tones, neon, monochrome)
- Texture details (materials, wear, aging)

**Example:** Add DOLLY-01 Slow Push-In:
```
Camera dolly forward 8 inches over 10 seconds (0.66 ft/sec),
imperceptible engagement, Steadicam smooth.
```

**Example:** Add STUDIO-02 Rembrandt Portrait:
```
Single key light positioned 45° above and 45° to side of subject creating
triangular highlight on shadow-side cheek (Rembrandt triangle). No fill or
minimal fill. 8:1 to 12:1 contrast.
```

---

## Layer 3: Style Preset (Overall Aesthetic)

**What it provides:**
- Complete color palette (specific hex codes)
- Overall lighting philosophy (approach and mood)
- Post-production treatment (grading, grain, vignette)
- Technical characteristics (resolution, artifacts, degradation)
- Mood/atmospheric direction
- Things to avoid for style consistency

**Example:** Film Noir Preset adds:
- Monochrome or -40% desaturation
- 16:1 to 25:1 extreme contrast
- Low-key dramatic lighting philosophy
- Crushed blacks, clipped highlights
- 25% film grain, dark vignette
- Noir mood: mystery, danger, moral ambiguity

---

# STEP-BY-STEP PROMPT BUILDING

## Example 1: Building a Product Showcase

**GOAL:** Luxury watch reveal video, 8 seconds, premium aesthetic

### Step 1: Choose Base Template

**Selected:** PRD-01 Clean Product Rotation
```
Reason: Need 360° product view, clean professional aesthetic
Provides: Rotation structure, clean background, lighting mentions
```

### Step 2: Add Modular Components

**Camera Movement:** LOCKED-01 Absolute Static
```
Camera locked on tripod, zero movement, absolute stability.
Product rotates, camera stays still (cleaner than orbit).
```

**Lighting Setup:** STUDIO-01 Three-Point Classic + modifications
```
Key light: Large soft box camera-left 45° for main illumination
Fill light: Soft panel camera-right at -2 stops preventing dark side
Rim light: Strip box top-back creating edge separation on metal
Background: Pure white separately lit
All 5600K LED balanced
```

**Color Palette:** COLOR-COM-01 Premium Luxury
```
Champagne Gold #F7E7CE accents
Deep Navy #1B2432 watch face
Bronze #CD7F32 hardware
Ivory #FFFFF0 background
Sophisticated muted saturation
```

**Texture Details:** TEX-SURF-02 Polished Chrome (for case)
```
Mirror-like reflective surface
Sharp specular highlights
Environment reflections visible
```

### Step 3: Apply Style Preset (Optional)

**Selected:** Modern Commercial Preset
```
High-key clean aesthetic
Commercial polish grade
Lifted shadows, preserved highlights
Slight saturation boost +10%
Remove all imperfections
```

### Step 4: Combine Into Final Prompt

```
FINAL ASSEMBLED PROMPT:

Photorealistic 360-degree product rotation of luxury Swiss watch suspended
in white void. Clean pure white background emphasizes elegant watch form.
Lighting reveals polished steel case and champagne gold accents through
carefully controlled specular highlights traveling across surface. Camera
locked on tripod maintains 15° elevated angle throughout rotation. Detailed
watch elements - sapphire crystal, guilloche dial, exhibition caseback -
remain visible and emphasized during rotation.

Shot on RED V-Raptor 8K, 8K resolution for maximum detail, 24fps. 85mm lens
at f/8.0, watch sharp throughout depth, background pure white void. Camera
locked absolute static on tripod, watch rotates on motorized turntable 45°
per second (360° in 8 seconds).

LIGHTING: Five-light studio setup - (1) Key: Large soft box camera-left 45°
creating main illumination and soft specular stripe on steel, (2) Fill: Soft
panel camera-right at -2 stops preventing dark side, (3) Rim: Strip light
creating highlight line on case edge for separation, (4) Dial accent: Small
focused spot highlighting champagne gold dial details, (5) Background: Two
lights creating pure white seamless #FFFFFF.

COLOR: Premium luxury palette - Polished steel case with mirror reflections,
champagne gold #F7E7CE dial, deep navy #1B2432 leather strap, bronze #CD7F32
hardware accents, pure white background #FFFFFF. Commercial polish grade:
slight saturation +10%, lifted shadows, preserved highlights.

ROTATION: Watch suspended on invisible monofilament, rotates clockwise 360°
over 8 seconds at constant 45°/second. Suspension point at watch balance
point creating stable rotation. Specular highlights travel across polished
surfaces during rotation revealing form.

MATERIAL RENDERING: Polished steel shows sharp specular highlights and
environment reflections, sapphire crystal has slight green tint at edges,
champagne gold dial catches light warmly, leather strap shows natural grain
texture, all materials rendered at premium quality with no fingerprints or
dust.

POST-PRODUCTION: Remove any suspension wire artifacts, ensure white
background absolute purity (255,255,255), highlight enhancement on gold
details, micro dust removal, commercial perfection.

Duration: 8 seconds exactly.

AVOID: Visible support, uneven rotation speed, harsh shadows, fingerprints,
background not pure white, clipped highlights on steel, camera drift.
```

---

## Example 2: Building a Documentary Interview

**GOAL:** Anonymous whistleblower interview, 10 seconds, serious credibility

### Step 1: Choose Base Template

**Selected:** DOC-02 Interview Subject
```
Reason: Interview setup structure, portrait framing guidance
Provides: Three-point light mention, MCU framing, basic structure
```

### Step 2: Add Modular Components

**Camera Movement:** LOCKED-01 Absolute Static
```
Interview standard - locked tripod, no drift, stable professional
```

**Lighting Setup:** NAT-03 North Window (Indirect)
```
Large north-facing window providing indirect daylight
Soft directional light 5000-5500K, no direct sun
White bounce card opposite window for fill at -1.5 stops
Natural but professional
```

**Composition:** COMP-01 Rule of Thirds
```
Subject positioned at right-third power point
Eyes on upper horizontal line
Look-space camera-left
```

### Step 3: Apply Style Preset

**Selected:** Naturalistic Documentary Preset
```
100% available light (matches window approach)
Minimal color correction
Authentic realism over beauty
Functional framing
```

### Step 4: Assemble Final Prompt

```
FINAL ASSEMBLED PROMPT:

Photorealistic documentary interview of whistleblower (35, female, business
casual) in office conference room. Subject positioned rule-of-thirds camera-
right at medium close-up responding to off-camera interviewer about
corporate misconduct. Natural serious expression conveys credibility and
concern without sensationalism. Background soft focus shows office
environment providing professional context.

Shot on Canon EOS R5, 4K, 24fps. 85mm lens at f/2.8, subject eyes sharp,
background office readable but soft. Locked tripod, eye-level perspective,
look-space camera-left where interviewer sits.

LIGHTING: 100% available light - Large north-facing window camera-right
provides natural key light (soft indirect daylight, 5200K), white bounce
card fill camera-left at -1.5 stops, no additional film lights. 5:1 natural
contrast, professional but documentary authentic.

COMPOSITION: Rule of thirds - Subject positioned right-third intersection,
eyes on upper horizontal line, look-space left for interviewer, background
office visible providing workplace context without distraction.

ENVIRONMENT: Corporate conference room, background shows office furniture
(soft focus), natural setting not staged, authentic workplace environment,
daylight from window suggests normal business hours.

COLOR: Minimal color correction - balance white for north window 5200K,
neutral saturation 0%, accurate skin tones not flattering, preserve
documentary objectivity. Slight desaturation -5% for serious tone.

SUBJECT: Female professional, 35, business casual attire (blazer, no tie),
direct eye contact with off-camera interviewer, serious engaged expression,
occasional subtle nods, professional composure with underlying concern,
credibility through authenticity.

POST: Documentary minimal intervention - balance color for window light,
level audio to -14 LUFS, preserve natural sensor characteristics, no beauty
enhancement, maintain professional credibility through authentic approach.

Duration: 10 seconds.

AVOID: Dramatic lighting, artificial beautification, staged background,
camera movement, performer emotion (needs authentic internal experience).
```

---

# 20 COMPLETE EXAMPLES

## EXAMPLE 1: Cyberpunk Street Scene

**Layers:**
- Base: ENV-02 Urban Environment (Night)
- Components: HANDHELD-02 Active Vérité, ATMO-05 Rain (Medium), COLOR-CIN-04 Cyberpunk Neon
- Style: Cyberpunk Preset

**Final Prompt:**
```
Photorealistic cyberpunk street scene, neon-saturated Tokyo Shibuya
intersection at night. Magenta #FF00FF and cyan #00FFFF LED billboards
create layered neon depth. Medium rain visible as diagonal streaks backlit
by neon, wet asphalt perfectly reflects vertical neon signs creating mirror
world below.

Shot on Sony A7S III, 4K, 24fps. 35mm lens at f/2.0, subject and foreground
sharp, background neon in colorful bokeh. Active handheld following
pedestrian with umbrella through crosswalk, reactive documentary energy.

LIGHTING: 100% practical neon sources - Magenta LED strips, cyan storefront
signs, electric blue #304FFE vertical billboards, orange #FF6600 vending
machines. Mixed color temperature chaos 2800K-8000K. Oversaturate neon +40%.

COMPOSITION: Eye-level immersed, pedestrian in middle ground with multiple
neon layers visible behind, vertical Japanese text signs frame edges.
Reflections in wet street create depth doubling.

ENVIRONMENT: Shibuya crossing, neon density overwhelming, rain creates wet
surfaces and atmospheric glow, steam rising from subway grates, mist around
brightest sources. Night always, urban saturation.

COLOR: Cyberpunk palette - Magenta #FF00FF, Cyan #00FFFF, Hot Pink #FF1744,
Electric Blue #304FFE on void black #0D0D0D. Oversaturate neon +40%, skin
tones desaturated -15%. Wet reflections preserve colors.

POST: Heavy teal-magenta split grade, glow bloom on brightest neon, slight
chromatic aberration 2px, minimal grain (modern digital).

Duration: 10 seconds.
```

---

## EXAMPLE 2: Vintage 1970s Product Commercial

**Layers:**
- Base: COM-01 Premium Product Hero
- Components: DOLLY-01 Slow Push-In, COLOR-NAT-01 Earth Tones
- Style: 1970s Film Stock Preset

**Final Prompt:**
```
Photorealistic 1970s product commercial aesthetic showcasing retro coffee
maker on warm wood surface. Warm earth tone palette: brown #8B4513 wood,
mustard #E8B923 product accent, avocado green #6B8E23 background. Film grain
30%, lifted blacks, vintage Kodak warmth.

Shot with vintage glass characteristics simulating 1970s cinema camera, 4K
downsampled, 24fps. 50mm lens at f/2.8 with slight soft focus diffusion 10%.
Slow dolly-in 6 inches over 8 seconds (0.75 ft/sec) toward product, gentle
engagement.

LIGHTING: Warm natural window light creating soft 5:1 contrast, gentle
modeling. Slight overexposure in highlights creating film glow acceptable.
3200K warmth overall.

ENVIRONMENT: 1970s kitchen counter, wood laminate surface, wallpaper
background in avocado green, period-appropriate styling.

COLOR: 1970s palette - Brown wood #8B4513, mustard yellow #E8B923, avocado
green #6B8E23. Desaturate -20%, warm +300K, slight green shift in shadows
(Kodak characteristic). Lifted blacks starting at level 10.

POST: Organic film grain 30%, lifted blacks not crushed, warm vintage tone,
slight green shadow shift, soft focus 10%, warm vignette 15%. Period
authentic not modern clean.

Duration: 8 seconds.
```

---

## EXAMPLE 3: Horror Found Footage (Analog VHS)

**Layers:**
- Base: ENV-02 Urban Environment (but modified for interior)
- Components: HANDHELD-04 Chaotic Energy, ATMO-01 Dust Motes in Light
- Style: Analog Horror Preset

**Final Prompt:**
```
VHS recording 1987, 480i resolution, visible horizontal scanlines 2px
spacing, tracking errors, chroma noise, analog static texture. Found footage
horror aesthetic abandoned hospital hallway exploration.

Photorealistic base then degraded to VHS quality. Handheld flashlight POV,
chaotic camera shake suggesting panic, aggressive 15mm displacement.
Flashlight beam creates dust mote visibility (heavy density 200 per cubic
foot), deep void blacks #0A0A0A beyond beam.

LIGHTING: Single handheld flashlight 3200K as only source, extreme contrast
25:1+, beam creates cone of light in darkness, dust particles dance in
beam. Occasional flicker suggesting battery weakness.

CAMERA: Chaotic handheld, aggressive shake, rapid uncontrolled reframes,
found footage panic aesthetic. Autofocus hunting (VHS characteristic).
Fixed 16mm perspective (consumer camcorder).

ENVIRONMENT: Abandoned hospital hallway, peeling institutional green paint
#7CB342, flickering overhead fluorescent (one tube), deep shadows, dust
accumulation, signs of abandonment. Cold 55°F implied.

COLOR: Desaturated -40% except phosphor green #33FF33 from distant exit
sign. VHS chroma bleeding at edges. Institutional green tint overall.

VHS DEGRADATION: Tracking errors 3-4 times creating horizontal tears, chroma
separation, generation loss blur, timestamp "11/23/1987 03:42 AM" white VCR
font lower-right.

AUDIO: Heavy breathing (panic), footsteps echoing, distant metallic clang,
fluorescent buzz, 60Hz hum, analog static -45dB.

Duration: 10 seconds of pure dread.
```

---

## EXAMPLE 4: High-End Fashion Editorial

**Layers:**
- Base: CHR-01 Emotional Portrait
- Components: NAT-01 Golden Hour Backlight, COMP-02 Golden Ratio
- Style: Modern Commercial Preset (modified for editorial)

**Final Prompt:**
```
Photorealistic high-fashion editorial portrait of model (20s, androgynous,
striking features) in dramatic pose. Golden hour backlight creates warm
3600K rim glow, face positioned at golden ratio spiral focal point. Deep
teal #16697A shadows contrast warm orange #FFA101 highlights (editorial
teal-orange grade).

Shot on ARRI Alexa LF, 4K, 24fps. 85mm T1.4 Signature Prime wide open,
razor-thin depth of field isolating face, background melts to soft bokeh.
Static locked composition, model holds pose with fierce confidence.

LIGHTING: Natural golden hour backlight 25 minutes before sunset positioning
sun behind subject creating warm rim light. Soft silver reflector fill
camera-left at -2.5 stops prevents silhouette. 8:1 dramatic contrast.

COMPOSITION: Golden ratio spiral focal point on model's leading eye, face
positioned at phi grid intersection. Asymmetrical but aesthetically perfect.
Negative space 40% of frame creating breathing room and elegance.

ENVIRONMENT: Desert location, out-of-focus sand dunes in background creating
warm orange bokeh. Heat shimmer visible in extreme background distance.

COLOR: Editorial grade - Deep teal #16697A shadows, warm orange #FFA101
highlights, strong complementary contrast. Skin tones warmed +200K, eyes
punched +20% saturation. Background desaturated -25% to emphasize subject.

FASHION: High-concept editorial styling, dramatic makeup, sculptural
silhouette, androgynous presentation, fierce energy.

POST: Editorial teal-orange grade, lifted shadows to teal, warm highlights,
skin retouching to editorial perfection (but maintain texture), slight film
grain 8% for editorial feel not sterile digital.

Duration: 8 seconds of held fierce gaze.
```

---

## EXAMPLE 5: Slow-Motion Water Impact

**Layers:**
- Base: CIN-04 Dynamic Action
- Components: MOTION-SPEED-04 Extreme Slow-Motion, LOCKED-01 Absolute Static
- Style: Minimalist/Clean Preset (for focus on physics)

**Final Prompt:**
```
Photorealistic water balloon impact on white surface shot at extreme slow-
motion. Captured 240fps conformed to 24fps playback (10x slow, 10% speed)
revealing balloon deformation, water explosion physics, droplet trajectories.
Pure white #FFFFFF background isolating subject, minimalist physics beauty.

Shot on Phantom Flex 4K high-speed camera, 4K, 240fps source. 100mm macro
lens at f/8.0, sufficient depth for explosion radius while maintaining
sharpness. Camera locked absolute static on tripod, subject motion only.

LIGHTING: High-key shadowless - Three large LED panels creating wrap-around
even illumination for high-speed capture (needs significant light output).
5600K daylight balanced. Background separately lit to pure white seamless.
2:1 minimal contrast emphasizing clean physics.

ACTION CHOREOGRAPHY (at 24fps playback):
0.0s: Balloon approaches surface (stretched teardrop)
1.5s: Initial contact, balloon deforms
2.5s: Balloon bursts, water begins explosive expansion
4.0s: Peak explosion, water radiates outward in crown shape
6.0s: Droplets at maximum dispersal, ballistic trajectories visible
8.0s: Droplets beginning descent, physics beauty peaks
10.0s: Water settling, aftermath visible

PHYSICS: Accurate water balloon physics at 10x slow-motion - balloon
deformation on impact, explosive burst pattern, crown splash formation,
individual droplet trajectories following ballistic curves, surface tension
visible, gravity affecting descent.

COLOR: Minimalist clean - transparent water with slight highlights, pure
white background #FFFFFF, minimal color. Clean digital aesthetic, no grain.

POST: Clean digital, no grain or artifacts, pure physics beauty. Slight
highlights enhancement on water droplets for visibility, otherwise
unprocessed realism.

Duration: 10 seconds playback (100 seconds real-time at 240fps).
```

---

## EXAMPLE 6: Film Noir Detective Scene

**Layers:**
- Base: CIN-02 Dramatic Portrait
- Components: STUDIO-06 Low-Key Noir, COMP-03 Centered Symmetry
- Style: Film Noir Preset

**Final Prompt:**
```
Photorealistic film noir detective portrait, hardboiled private investigator
(50s, male, worn trench coat, fedora) at office desk illuminated by single
desk lamp. Monochrome palette, crushed blacks #000000, hot whites #FFFFFF,
extreme contrast 20:1. Venetian blind slash shadows across face and wall.

Shot on ARRI Alexa Mini LF, 4K, 24fps. 85mm T2.1 at f/2.8, face sharp, deep
shadows impenetrable. Static locked low angle looking slightly up at
subject, centered symmetrical composition creating formal power.

LIGHTING: Single hard tungsten desk lamp 2900K as only source creating
dramatic shadows. Positioned 45° camera-right and low creating shadows
upward. No fill light, deep blacks dominate frame. Venetian blind off-
screen creating slash patterns across back wall. 20:1 extreme contrast.

COMPOSITION: Centered symmetry - Subject positioned dead center creating
formal power and noir formality. Cigarette smoke visible in desk lamp beam
creating volumetric depth. Negative space darkness surrounds subject.

ENVIRONMENT: 1940s private detective office, desk lamp illuminates
immediate area only, venetian blind shadows on back wall, darkness beyond
light radius. Cold noir atmosphere, night time.

COLOR: Full monochrome or desaturated -60%. Blacks crushed to pure #000000,
highlights clipped to hot white #FFFFFF. Shadows cold blue #2C3E50, desk
lamp warm orange #FF8C00 tint. Film noir palette absolute.

CHARACTER: Private detective archetype, weathered face showing years,
cigarette smoke curling, direct gaze at camera (breaks fourth wall
intentionally), fedora shadow across eyes, moral ambiguity visible.

POST: Film noir grade - desaturate -60% or full B&W, crush blacks to level
0, clip highlights to 250, +40% midtone contrast, 25% film grain, 25% dark
vignette, cold shadows warm highlights split.

Duration: 8 seconds of noir atmosphere.

AVOID: Bright lighting, warm tones, color, soft shadows, modern aesthetic.
```

---

## EXAMPLE 7: Nature Documentary Landscape

**Layers:**
- Base: ENV-01 Natural Landscape (Wide)
- Components: AERIAL-01 Drone Ascent, WEATHER-05 Golden Hour Clear
- Style: Naturalistic Documentary Preset

**Final Prompt:**
```
Photorealistic wide natural landscape of Norwegian fjord at golden hour
clear conditions. Warm 3800K sunlight 25 minutes before sunset creating long
shadows and golden glow. Drone slow ascent 60 feet over 12 seconds revealing
dramatic vertical cliff scale and pristine wilderness.

Shot on DJI Inspire 3, 8K, 24fps. 24mm equivalent lens at f/11, deep depth
maintaining sharpness from foreground water to distant peaks 3 miles away.
Autonomous drone ascent perfectly smooth, 5 ft/sec constant.

LIGHTING: Natural golden hour clear sky - Direct sun from camera-left
creating warm 3800K key light, open sky soft fill, long dramatic shadows.
Mountain peaks catching warm alpenglow. Natural 8:1 contrast.

COMPOSITION: Three-plane depth - Foreground fjord water surface (0-100ft),
middle distance vertical granite cliffs emerging (100-2000ft), background
snow-covered peaks (2000ft-5000ft). Leading lines from water edges toward
distant peaks.

ENVIRONMENT: Norwegian fjord wilderness, pristine nature, no human
structures visible, clear golden hour sky, slight early morning mist in
valleys. Autumn season (golden foliage accents on ledges).

COLOR: Natural accurate colors - Deep blue water #1A3A52, granite gray
#6E7F80, autumn gold foliage #FFB627, snow white peaks, warm golden hour
glow overall. Minimal grading, preserve natural beauty. Neutral saturation
0% or slight -5%.

CAMERA MOVEMENT: Drone begins 40 feet above water surface showing
foreground, ascends straight up 60 feet over 12 seconds, final altitude
shows full scope of fjord depth and cliff scale. Smooth autonomous flight.

POST: Documentary minimal - natural color balance for golden hour 3800K,
preserve authentic wilderness colors, no artistic grading, slight -5%
desaturation for documentary objectivity, no grain (clean digital).

Duration: 12 seconds of natural majesty.

AVOID: Artistic color grading, time-lapse speed, HDR unrealism, visible
drone shadow, human structures in frame.
```

---

## EXAMPLE 8: Tech Product Launch Reveal

**Layers:**
- Base: PRD-02 Exploded Assembly View
- Components: COLOR-COM-02 Tech/Innovation, MOTION-SPEED-02 Subtle Slow-Motion
- Style: Modern Commercial Preset

**Final Prompt:**
```
Photorealistic smartphone exploding into 47 component parts showing internal
engineering innovation. Shot at 48fps conformed to 24fps (2x slow, 50%
speed) creating subtle slow-motion elegance. Components float apart radially
revealing processor, camera array, battery, display layers. Clean white
#FFFFFF to cool gray #E8E8E8 gradient background. Tech innovation aesthetic.

Shot on RED Komodo 6K, 6K, 48fps source. 85mm lens at f/8.0, sufficient
depth to keep near and far components acceptably sharp. Static locked
camera, components move via animation.

LIGHTING: High-key technical - Six LED panels creating shadowless
illumination for clarity. 5600K daylight balanced. Each component clearly
lit regardless of position. White gradient background separately lit.

EXPLOSION CHOREOGRAPHY (12s at 50% playback):
0.0-2.0s: Assembled phone, complete
2.0-4.0s: Display lifts away first
4.0-6.0s: Internal components begin separating radially
6.0s: Full explosion, all 47 parts suspended in space
6.0-10.0s: Parts hover, slowly rotate showing detail
10.0-12.0s: Hold expanded state, camera subtle push-in

COMPONENT ORGANIZATION: Parts separate along functional groups - Display
components up, processor/logic board center, battery down, camera module
back-left, case components outward radially. Organized explosion not chaos.

COLOR: Tech innovation palette - Clean white #FFFFFF base, cool gray #E8E8E8
surfaces, accent blue #0066FF highlights on key components (processor,
camera), polished metal #C0C0C0, matte black #2C2C2C. Modern clean aesthetic.

TECHNICAL DETAILS: Visible engineering - layered logic board traces, camera
lens array, battery cells, antenna lines, precision component placement,
modern smartphone complexity visualization.

POST: Modern commercial polish - clean no grain, lifted shadows, precise
color control, slight saturation +10% on accent blue, component labels
optional (text overlays), pristine digital aesthetic.

Duration: 12 seconds at 50% playback.
```

---

## EXAMPLE 9: Gritty Street Documentary

**Layers:**
- Base: DOC-04 Vérité Action
- Components: HANDHELD-02 Active Vérité, WEATHER-04 Rain Wet Streets
- Style: Gritty Realism Preset

**Final Prompt:**
```
Photorealistic gritty street documentary following delivery worker through
rainy urban night. Desaturated -35%, harsh sodium vapor street light 2200K,
wet streets reflecting orange glow. Active handheld reactive camera following
subject through frame, authentic documentary chaos.

Shot on Panasonic S1H documentary setup, 4K, 24fps. 35mm lens at f/4.0,
continuous autofocus handling variable distance. Handheld shoulder rig,
organic operator shake and breathing visible.

LIGHTING: 100% available street lighting - Sodium vapor street lamps 2200K
creating harsh orange key, fluorescent storefront 4100K providing cool fill,
occasional car headlights 5000K. Mixed color temperature chaos. High
contrast 12:1 with deep unflattering shadows. No added light.

CAMERA MOVEMENT: Active handheld following delivery worker on bicycle,
reactive not predictive, operator jogs alongside maintaining rough framing,
occasional soft focus during fast reframes (authentic mistake preserved),
slight frame corrections visible, documentary immediacy.

ENVIRONMENT: Working-class urban neighborhood night, wet streets from
earlier rain creating reflections, puddles on broken pavement, graffiti
visible on shuttered storefronts, real location chaos not cleaned.

COLOR: Heavy desaturation -35%, gritty palette: rust orange from sodium
vapor, concrete gray #808080, asphalt black wet and reflective. Mixed color
temps preserved showing realistic chaos. Skin tones unflattering slight
green cast.

SUBJECT: Delivery worker (30s, male, reflective vest over hoodie, backpack)
navigating wet streets, authentic labor, unaware of camera or accepting
presence, real work pace not performed.

WEATHER: Post-rain wet streets mandatory, puddles reflect street lights,
asphalt dark wet creating reflective mirror, occasional splash from bike
tire through puddle, mist visible in light beams.

POST: Gritty grade - desaturate -35%, increase grain 25% (16mm documentary
feel), lift blacks to 15 (crushed floor), increase midtone contrast +20%,
preserve authentic imperfections and camera shake.

Duration: 15 seconds of urban realism.

AVOID: Beauty lighting, clean backgrounds, smooth camera, saturated colors,
glamorization, removed imperfections.
```

---

## EXAMPLE 10: Dreamlike Memory Sequence

**Layers:**
- Base: CHR-03 Gesture/Hand Performance (modified)
- Components: MOTION-SPEED-06 Speed Ramp, NAT-01 Golden Hour Backlight
- Style: Dreamlike/Surreal Preset

**Final Prompt:**
```
Photorealistic dreamlike sequence of elderly hands sorting old photographs,
soft pastel glow, gentle slow-motion feel. Shot 30fps conformed to 24fps
(75% speed) creating suspended time quality. Soft lavender #E6E6FA and
peach #FFDAB9 color palette, overexposed highlights blooming white.

Shot on Sony VENICE 2, 4K, 30fps source. 85mm T2.1 at f/2.0, hands sharp,
photographs in moderate focus, background soft ethereal bokeh. Slow floating
Steadicam drift creating weightless dreamy movement.

LIGHTING: Soft golden hour backlight through sheer curtains creating warm
3600K glow and soft halo. Large white reflector fill preventing
silhouette. Low contrast 3:1, soft shadows, blooming highlights acceptable
(dream aesthetic not technical perfection). Overexposure +1 stop creating
ethereal glow.

COMPOSITION: Close-up overhead angle looking down at hands and photographs
spread on table. Soft edges, blooming highlights from window, negative
space glowing white. Grandmother's hands (80s, age spots, wedding ring worn
thin) sorting through color photographs from 1970s.

ENVIRONMENT: Soft-focus living room, afternoon light through sheer curtains,
dust motes visible in backlight beam creating fairy-dust quality. Warm
nostalgic atmosphere.

COLOR: Soft pastel desaturation -15%, warm overall +400K. Lavender #E6E6FA
shadows, peach #FFDAB9 highlights, cream #FAF9F6 blooming whites.
Photographs show faded 1970s colors (Kodak warm tones). Gentle color
gradients throughout.

MOTION: Hands move slowly and gently, captured at 30fps played at 24fps =
75% gentle slow-motion. Time feels suspended, movements dreamlike. Speed
ramp to 50% at key moment (touching specific photograph), return to 75%.

POST: 15% soft diffusion/glow filter, bloom highlights to white ethereal
glow, lift shadows to level 20 (no deep blacks), desaturate -15%, warm
grade +400K creating nostalgic dream warmth, minimal grain (clean dream).

Duration: 10 seconds playback (13 seconds real-time at 75% speed).

MOOD: Memory, nostalgia, time passing gently, dream state, warm
reminiscence, soft sadness, beauty in age, suspended moment.
```

---

*[Continue with Examples 11-20...]*

## EXAMPLE 11: Minimalist Architecture Detail

**Base:** ENV-03 (create as architectural interior)
**Components:** COMP-06 Negative Space, COLOR Monochrome
**Style:** Minimalist/Clean Preset

```
Photorealistic minimalist architectural detail of concrete staircase in
white void. Subject (staircase) occupies 20% of frame lower-right, remaining
80% pure white #FFFFFF negative space emphasizing geometric form and minimal
aesthetic.

Shot on Phase One IQ4 (architectural detail), 100MP, static locked tripod.
35mm tilt-shift lens at f/11, deep focus maintaining architectural line
sharpness. Perfectly level camera, zero movement.

LIGHTING: Even shadowless illumination - Soft diffused overhead creating
2:1 minimal contrast. Concrete texture visible but gentle. No harsh shadows,
geometric form revealed through edge definition not dramatic lighting.

COMPOSITION: Negative space dominant - Staircase positioned lower-right rule
of thirds, 80% of frame empty white void. Geometric precision, clean lines,
minimal aesthetic. Diagonal stair geometry creates only visual energy.

ENVIRONMENT: Pure white void studio, no context visible, staircase as
sculptural object isolated from architectural function. Zen minimal.

COLOR: Monochrome minimal - Concrete gray #808080, pure white void #FFFFFF.
No color, geometric form and negative space as only visual elements.
Desaturated -100% full monochrome.

POST: Clean digital perfection - no grain, no artifacts, pure geometric
precision. Exact color control, pure white background maintained, slight
contrast in midtones to show concrete texture subtly.

Duration: 8 seconds of minimal contemplation.
```

---

## EXAMPLE 12: Fantasy Magic Ritual Scene

**Base:** CIN-05 Atmospheric Mood
**Components:** SPEC-04 Fire/Flame Practical, ATMO-02 Light Fog/Mist
**Style:** Fantasy/Magical Preset

```
Photorealistic fantasy ritual scene, robed figure performing magic ceremony
in ancient stone chamber. Multiple candles (20+) providing warm 2400K
flickering light creating volumetric god rays through atmospheric mist.
Rich saturated jewel tones: deep purple #4B0082 robe, gold #FFD700 runic
circle, emerald #50C878 magical energy glow.

Shot on ARRI Alexa 65, 4K, 24fps. 35mm lens at f/2.8, selective focus on
figure with background candles creating warm bokeh. Slow dolly-in 10 inches
over 12 seconds approaching ritual.

LIGHTING: Multiple candle practicals creating warm 2400K base, organic
flicker 3-5Hz irregular. LED panel provides subtle cyan #7FDBFF magical
energy glow from runic circle on floor. Volumetric mist makes light beams
visible creating god rays through chamber. 10:1 dramatic contrast.

COMPOSITION: Wide establishing beginning, slow dolly approach. Figure
positioned center of runic circle, candles arranged in ritual pattern,
ancient stone archways frame edges. Depth through atmospheric haze layers.

ENVIRONMENT: Ancient stone chamber, weathered walls, carved runic symbols
visible in candlelight, atmospheric mist reducing visibility to 300 feet
creating mystical depth. Medieval fantasy atmosphere, timeless magic.

COLOR: Rich fantasy saturation +20% - Deep purple robe #4B0082, gold runic
circle #FFD700, emerald magical energy #50C878, warm candlelight amber,
stone gray. Shadows maintain color not pure black. Glowing bloom on magical
elements.

MAGICAL ELEMENTS: Runic circle glows cyan-green from floor, candle flames
dance in pattern suggesting unseen energy, mist swirls subtly around figure,
volumetric light creates supernatural atmosphere. Fantasy physics.

POST: Rich grade +20% saturation, glowing bloom on candles and runic
elements, volumetric light enhancement, film grain 15% (organic not sterile),
warm candle tint throughout, deep shadows with retained color.

Duration: 12 seconds of magical ritual.
```

---

## EXAMPLE 13: 1980s VHS Home Video

**Base:** DOC-01 Observational Wide (modified for home video)
**Components:** Multiple VHS technical characteristics
**Style:** 1980s VHS Preset

```
VHS recording December 1985, 480i resolution, visible horizontal scanlines
2px spacing, chroma noise, color bleeding, oversaturated +40%. Home video
aesthetic family Christmas morning living room.

Consumer camcorder perspective, slight handheld shake (operator unfamiliar
with equipment), occasional autofocus hunting, reactive zoom usage (amateur
videographer). 4:3 aspect ratio.

LIGHTING: Available home lighting - Christmas tree lights creating warm
colored practicals, overhead living room lights harsh fluorescent mixed with
tungsten table lamps. Mixed color temperature chaos from auto white balance
failures. High contrast 10:1 typical of video.

ENVIRONMENT: 1985 living room authenticity - Wood paneling walls, shag
carpet, period-appropriate furniture, wrapped presents under tree,
wallpaper, analog TV visible in background showing static, rotary phone on
end table.

COLOR: VHS oversaturation +40%, slight magenta cast overall. Christmas tree
lights creating colored flares (red, green, blue bleeding). Electric blue,
hot magenta primaries. Chroma separation at color edges visible.

VHS TECHNICAL: Tracking errors 2-3 times creating horizontal tears, reduced
sharpness from generation loss, chroma noise at edges, date stamp lower
right "DEC 25 1985" white VCR OSD font, slight ghosting on motion.

CAMERA: Consumer handheld camcorder feel - Slight shake, reactive zoom
toward action (child opening present), autofocus hunting briefly when zoom
occurs, amateur framing slightly off-center. Real family videographer not
professional.

AUDIO: VHS audio compression, family voices slightly distorted, background
Christmas music from radio tinny, children excitement, paper tearing,
ambient home sounds. Mono audio centered.

Duration: 15 seconds of nostalgic home video.

AVOID: Clean digital, perfect color, smooth professional camera work, modern
aesthetics, HD resolution feel.
```

---

## EXAMPLE 14: High-Speed Product Splash

**Base:** CIN-04 Dynamic Action
**Components:** MOTION-SPEED-04 Extreme Slow-Motion, STUDIO-05 High-Key Commercial
**Style:** Modern Commercial Preset

```
Photorealistic high-speed product shot of fresh fruit (strawberry) splashing
into water creating crown splash and droplet spray. Captured 240fps
conformed to 24fps (10x slow-motion, 10% speed). Clean white #FFFFFF
background, commercial high-key aesthetic. Water physics frozen in detail.

Shot on Phantom Flex 4K, 4K, 240fps. 100mm macro at f/8.0, strawberry and
splash sharp, background pure white. Static locked camera, subject action
only.

LIGHTING: High-key commercial setup for high-speed - Four large LED panels
wrap-around creating shadowless illumination (needed for 240fps light
requirements). 5600K balanced. Background separately lit to pure white.
2:1 minimal contrast, clean commercial aesthetic.

SPLASH CHOREOGRAPHY (10s playback = 100s real-time):
0.0s: Strawberry approaches water surface
1.5s: Initial contact, surface tension breaks
3.0s: Crown splash begins forming
5.0s: Peak crown splash, water droplets at maximum height
7.0s: Droplets follow ballistic curves downward
9.0s: Secondary splashes from droplet impacts
10.0s: Water settling, strawberry submerged

PHYSICS: Accurate water splash physics at 10x slow-motion - Crown splash
formation, individual droplet trajectories, surface tension visible, light
refraction through water, gravity effects on droplets, secondary impact
ripples.

COLOR: Clean commercial - Strawberry red #C1440E at vibrant saturation
+20%, water transparent with highlights, pure white background #FFFFFF,
minimal color palette emphasizing fresh product.

POST: Commercial clean - No grain, pristine digital, slight highlights boost
on water droplets for visibility, strawberry color enhanced +20%, background
absolute white (255,255,255).

Duration: 10 seconds playback.

AVOID: Dirty water, cluttered background, insufficient lighting creating
motion blur, strawberry imperfections visible.
```

---

## EXAMPLE 15: Noir Crime Scene Investigation

**Base:** DOC-03 Detail Close-Up (Evidence)
**Components:** SPEC-05 Single Candle Darkness, COMP-04 Frame Within Frame
**Style:** Film Noir Preset

```
Photorealistic film noir crime scene detail, detective's gloved hand holding
magnifying glass examining evidence on desk. Single desk lamp provides only
illumination creating extreme 25:1 contrast. Monochrome -60%, crushed blacks,
venetian blind shadows across scene. Evidence framed within magnifying glass
creating frame-within-frame composition.

Shot on ARRI Alexa Mini, 4K, 24fps. 85mm macro at f/2.8, magnifying glass
contents sharp, background falls to dark bokeh. Static locked low angle,
dutch tilt 15° creating unease.

LIGHTING: Single hard desk lamp 2900K as only source positioned 90° camera-
left creating harsh directional light. Extreme contrast 25:1, no fill, deep
impenetrable blacks dominate. Venetian blind off-screen creates slash
shadow patterns across desk surface.

COMPOSITION: Frame-within-frame - Magnifying glass creates circular frame
around key evidence (photograph, bullet casing, note). Detective's hand
enters from frame edge. Dutch angle 15° adds tension. Negative space
darkness surrounds lit area.

ENVIRONMENT: 1940s detective office desk, evidence scattered, cigarette
smoke visible in desk lamp beam creating volumetric quality, darkness beyond
light radius absolute. Night time, noir atmosphere heavy.

COLOR: Monochrome or desaturated -60%. Blacks crushed to pure #000000,
highlights hot white. Desk lamp warm orange #FF8C00 tint, shadows cold blue
#2C3E50. Film noir absolute.

DETAIL: Evidence visible through magnifying glass enlarged - photograph
showing suspect, handwritten note partially visible, brass bullet casing
catching light. Detective's leather glove texture visible, weathered hands.

POST: Noir grade - desaturate -60%, crush blacks to level 0, clip highlights
to 250, +40% midtone contrast, 25% film grain, 25% dark vignette, venetian
blind shadow overlay.

Duration: 8 seconds investigating evidence.
```

---

## EXAMPLE 16: Naturalistic Cooking Process

**Base:** DOC-03 Detail Close-Up (Evidence) modified
**Components:** NAT-03 North Window, MOTION-SUBJ-01 Slow Deliberate
**Style:** Naturalistic Documentary Preset

```
Photorealistic documentary close-up of hands preparing traditional pasta,
flour dusting marble surface, slow deliberate movements showing generations
of skill. Natural north window light creating soft illumination. Minimal
color grading preserving authentic kitchen reality.

Shot on Blackmagic Pocket 6K, 4K, 24fps. 85mm macro at f/4.0, hands and
pasta sharp, background kitchen in soft focus. Locked tripod overhead 45°
angle looking down at work surface.

LIGHTING: 100% natural north window light from camera-left providing soft
key 5200K, white reflector fill camera-right at -1.5 stops. 5:1 natural
contrast, gentle modeling, no artificial lights. Authentic kitchen natural
illumination.

MOTION: Hands move slowly deliberately 0.7 ft/sec, each movement intentional
showing craft mastery. Flour dusting, dough kneading, pasta rolling -
movements complete fully before next begins. Contemplative rhythm showing
skill and care.

ENVIRONMENT: Home kitchen, marble work surface, wooden rolling pin,
scattered flour, authentic cooking workspace not staged. Background shows
real kitchen context (stove, utensils) soft focus.

COLOR: Minimal natural color correction - Balance for north window 5200K,
neutral saturation 0%, authentic ingredient colors. Flour white, pasta dough
cream, marble surface natural gray. Preserve documentary authenticity -5%
slight desaturation only.

HANDS: Elderly hands (70s, female), age spots visible, flour dusting fingers,
wedding ring worn, decades of cooking evident in confident movements. Real
skill not performed, authentic technique.

POST: Documentary minimal - Natural color balance, level exposure, preserve
natural sensor characteristics, no beauty enhancement, maintain ingredient
and skill authenticity through minimal intervention.

Duration: 10 seconds of meditative craft.

AVOID: Dramatic lighting, color grading beauty, staged perfect ingredients,
rapid movement, artificial enhancement.
```

---

## EXAMPLE 17: Cyberpunk Hacker Den

**Base:** ENV-02 Urban Environment (Night) modified for interior
**Components:** SPEC-03 Motivated Neon/Colored Practical, ATMO-04 Smoke/Haze
**Style:** Cyberpunk Preset

```
Photorealistic cyberpunk hacker workspace, figure silhouetted against wall
of monitors displaying scrolling code. Multiple colored LED strips creating
neon atmosphere: magenta #FF00FF, cyan #00FFFF, electric blue #304FFE.
Atmospheric haze making light beams visible. Void black #0D0D0D base,
oversaturated neon +40%.

Shot on Sony A7S III (low-light specialist), 4K, 24fps. 35mm at f/2.0,
monitor glow and figure sharp, background neon in soft bokeh. Static locked
camera emphasizing density of tech.

LIGHTING: 100% practical colored sources - Magenta LED strip camera-left,
cyan LED strip camera-right, electric blue monitor glow as fill, multiple
small indicator LEDs creating depth. Mixed color temperature 2800K-8000K.
Oversaturate all neon +40%. Figure backlit creating silhouette with colored
rim lights.

COMPOSITION: Figure silhouetted center-right, wall of monitors behind
creating background density, foreground keyboard and mouse catching colored
underglow. Layered tech depth, cables creating organic chaos against neon
geometry.

ENVIRONMENT: Small room/closet converted to hacking den, walls covered in
monitors, cable management chaos visible, empty energy drink cans, darkness
outside visible tech bubble. Underground tech aesthetic.

COLOR: Cyberpunk neon palette - Magenta #FF00FF, Cyan #00FFFF, Electric
Blue #304FFE, Hot Pink #FF1744 accents on void black #0D0D0D. Oversaturate
neon +40%, skin tones desaturated -20%. Monitor text green #00FF00 phosphor.

ATMOSPHERE: Light atmospheric haze making LED strips create visible beams,
cigarette or vape smoke adding to atmosphere, dust particles in colored
light. Tech den density and saturation.

POST: Heavy teal-magenta split grade, neon bloom/glow on brightest sources,
slight chromatic aberration 2px, minimal grain (modern digital), punched
saturation on all colored sources.

Duration: 10 seconds of hacker aesthetic.
```

---

## EXAMPLE 18: Golden Age Hollywood Glamour

**Base:** CHR-01 Emotional Portrait
**Components:** STUDIO-03 Butterfly/Paramount, COLOR-CIN-05 Vintage Film Stock
**Style:** Modified Modern Commercial with vintage treatment

```
Photorealistic golden age Hollywood glamour portrait, classic beauty (30s,
female, marcel waves, red lips) in dramatic pose. Butterfly glamour lighting
creating symmetrical nose shadow, soft focus diffusion 15%, warm vintage
film tones. 1940s studio portrait aesthetic.

Shot on ARRI Alexa 65 with vintage glass (Cooke Panchro), 4K, 24fps. 85mm
T2.3 with additional 15% soft focus diffusion filter. Static locked
composition, subject holds glamour pose.

LIGHTING: Classic Hollywood butterfly setup - Large overhead softbox
centered 40° above subject creating symmetrical butterfly shadow under nose.
Large white reflector below face provides glamour fill from underneath
(removes under-eye shadows). Rim lights camera-left and camera-right
creating hair separation. 3:1 soft flattering contrast hiding texture.

COMPOSITION: Classic Hollywood centered portrait, symmetrical composition
creating formal glamour. Subject direct gaze at camera, chin slightly down
(glamour angle), shoulders angled creating elegant line. Negative space
minimal, subject dominates frame.

ENVIRONMENT: Seamless gray background gradient, classic studio portrait,
no environmental context, timeless glamour isolation.

COLOR: Vintage Hollywood warmth - Champagne gold #F7E7CE highlights, warm
skin tones +300K, deep burgundy #800020 lips, sepia shadow tint. Kodak warm
vintage film stock emulation. Slight desaturation -15% creating elegance.

STYLING: 1940s authentic - Marcel wave hairstyle, classic red lipstick,
defined eyebrows, elegant jewelry, period-appropriate glamour not modern
beauty standards.

POST: Vintage Hollywood treatment - 15% soft focus diffusion, warm grade
+300K, sepia tint in shadows, lifted blacks to level 15 (vintage film
characteristic), 20% organic film grain, slight vignette 15% warm edges.

Duration: 8 seconds of timeless glamour.

AVOID: Modern sharp digital, harsh lighting, contemporary makeup, cold
color temperature, visible texture/pores.
```

---

## EXAMPLE 19: Abstract Paint Fluid Dynamics

**Base:** ART-01 Abstract Motion
**Components:** MOTION-SPEED-04 Extreme Slow-Motion, LOCKED-01 Absolute Static
**Style:** Minimalist/Clean Preset (for abstract focus)

```
Photorealistic abstract visualization of ink droplets (cyan, magenta, yellow)
mixing in water at extreme slow-motion. 240fps conformed to 24fps (10x slow,
10% speed) revealing fluid dynamics, turbulent diffusion patterns, color
mixing emergence. White #FFFFFF background creating clean field for color
interaction.

Shot on Phantom Flex 4K, 4K, 240fps. 100mm macro at f/8.0, water surface
impact sharp, sufficient depth for bloom pattern. Static locked camera,
subject fluid motion only.

LIGHTING: High-key setup for high-speed photography - Three LED panels
creating even illumination through clear water tank, backlight from behind
tank creating glow and color saturation, overhead for surface definition.
All 5600K. High intensity for 240fps frame rate.

SETUP: Clear glass tank 12"x12"x12" filled with purified water, white
background 12" behind, ink droplets (water-soluble) in CMY primaries: Cyan
#00FFFF, Magenta #FF00FF, Yellow #FFFF00. Dropped from 18" using precision
pipette.

FLUID CHOREOGRAPHY (10s playback = 100s real-time):
0.0s: Cyan droplet approaches surface (spherical)
1.0s: Impact, crown splash forms, surface tension breaks
2.0s: Cavity formation, droplet penetrates
3.0s: Turbulent diffusion creates bloom tendrils
4.0s: Magenta droplet impacts, colors begin mixing
5.0s: Cyan+Magenta tendrils intertwine creating blue where they meet
7.0s: Yellow droplet enters, three-color interaction
9.0s: Secondary colors emerge (blue, green, red-orange) from subtractive
     mixing
10.0s: Complex organic flow patterns, colors continuing diffusion

ABSTRACT FOCUS: Frame crops to show only color and form, tank edges not
visible, scale ambiguous, pure visual experience divorced from "ink in
water" literal reading. Emphasis on emergent complexity from simple physics.

COLOR: Pure CMY primaries at input saturated +30%, secondary colors emerge
naturally from mixing (blue, green, orange), white background absolute
#FFFFFF providing neutral contrast field.

POST: Clean abstract - No grain, pure digital, preserve physically-created
colors without adding non-existent hues, slight saturation +30% for visual
impact, white background maintained pure.

Duration: 10 seconds playback (100 seconds real-time).

AVOID: Artificial color addition in post, symmetrical mixing patterns,
visible container, editing cuts breaking flow.
```

---

## EXAMPLE 20: Post-Apocalyptic Survivor Portrait

**Base:** CHR-01 Emotional Portrait
**Components:** NAT-04 Direct Sun Hard Light, COMP-DYN-03 Dutch Angle
**Style:** Gritty Realism Preset

```
Photorealistic post-apocalyptic survivor portrait, weathered face (40s,
gender-neutral, scarred, dust-covered) against harsh desert wasteland. Direct
midday sun creating brutal 18:1 contrast, deep unflattering shadows. Dutch
angle 25° creating unease and instability. Desaturated -40%, rust and dust
palette.

Shot on RED V-Raptor, 4K, 24fps. 85mm at f/4.0, face sharp, desert wasteland
background in moderate focus showing devastation context. Handheld subtle
shake suggesting documentary observation in harsh conditions.

LIGHTING: Direct harsh midday sun 5400K creating hard dramatic shadows under
eyes, nose, cheekbones. 18:1 extreme contrast, no fill (survival reality
not beauty), squinting from sun brightness, harsh unflattering reality.
Overhead sun position creating worst possible portrait lighting
intentionally.

COMPOSITION: Dutch angle 25° creating instability and unease. Subject
positioned right-third with look-space left toward wasteland. Tight framing,
environmental devastation visible but secondary to human survival story.

ENVIRONMENT: Desert wasteland background, rust-colored sand, destroyed
infrastructure visible in distance (collapsed power lines, burned vehicles),
heat shimmer from sand, harsh survival reality. Post-apocalyptic devastation
context.

COLOR: Heavy desaturation -40%, rust #B7410E and dust palette, concrete gray
#808080, dirt brown #654321. Skin tones unflattering with sun-damage visible,
slight red sunburn, dust accumulation in creases. Gritty reality palette.

CHARACTER: Survival evidence visible - scarred face, sun damage, squinting
from brightness, dust/dirt accumulated, improvised clothing, thousand-yard
stare showing psychological toll, no performance only survival weariness.

POST: Gritty grade - desaturate -40%, increase grain 30% (harsh environment),
lift blacks to 20 (dusty atmosphere), increase midtone contrast +25%
(harsh sun), preserve all imperfections showing survival reality.

Duration: 8 seconds of survivor testimony.

AVOID: Beauty lighting, clean subject, saturated colors, level horizon
(needs dutch angle unease), staged performance emotion.
```

---

# TROUBLESHOOTING COMMON ISSUES

## Issue: Generated video lacks specificity

**Problem:** Sora 2 interprets prompt too generally, generic result

**Solutions:**
1. Add specific measurements and quantities
   - Instead of: "Many candles"
   - Use: "20 candles arranged in ritual circle pattern"

2. Include precise color hex codes
   - Instead of: "Blue and orange lighting"
   - Use: "Cyan #00FFFF key light, orange #FF6600 rim light"

3. Specify exact timing/duration
   - Instead of: "Camera moves toward subject"
   - Use: "Camera dolly forward 8 inches over 6 seconds (1.33 inches/sec)"

4. Define materials and textures explicitly
   - Instead of: "Metal surface"
   - Use: "Brushed aluminum with linear grain pattern, specular highlights
     elongating along grain direction"

---

## Issue: Camera movement feels wrong

**Problem:** Movement doesn't match intention or feels unnatural

**Solutions:**
1. Specify exact speed in ft/sec or inches/sec
2. Name movement type explicitly (dolly, crane, Steadicam, handheld)
3. Add movement quality descriptors (smooth, organic, chaotic, mechanical)
4. Include start and end positions clearly
5. Consider using "static" if movement creates issues

---

## Issue: Lighting doesn't match vision

**Problem:** Generated lighting too flat, too harsh, or wrong mood

**Solutions:**
1. Specify contrast ratio explicitly (3:1 soft, 20:1 dramatic)
2. Name exact lighting setup from library (Rembrandt, butterfly, practical-only)
3. Include color temperature in Kelvin (2700K warm, 5600K neutral, 7500K cool)
4. Describe light quality (hard/soft, directional/diffused)
5. Mention specific equipment (softbox, fresnel, practical lamp)

---

## Issue: Colors don't match expectation

**Problem:** Generated colors wrong saturation, temperature, or palette

**Solutions:**
1. Use hex codes for critical colors (#FF0000 not "red")
2. Specify saturation adjustment (+20% or -30%)
3. Include color temperature (3200K warm, 6500K neutral, etc.)
4. Reference established palette from Color Library by name
5. Describe color relationships (complementary, analogous, monochrome)

---

## Issue: Subject/environment too generic

**Problem:** Lacks specific details that make scene unique

**Solutions:**
1. Add period-specific details (1987 technology, 1940s furniture)
2. Include wear/aging characteristics (rust, patina, scratches)
3. Specify exact environmental elements (fluorescent overhead, neon signs)
4. Describe materials explicitly (concrete, brass, full-grain leather)
5. Add human-scale objects for reference

---

## Issue: Motion feels wrong speed

**Problem:** Action too fast, too slow, or wrong rhythm

**Solutions:**
1. Specify frame rate capture and playback explicitly
   - "Shot 120fps, playback 24fps = 5x slow-motion (20% speed)"
2. Use Motion Speed descriptors from library
3. Include physics references (gravity 9.8 m/s², realistic fall speed)
4. Describe rhythm/pacing (contemplative, urgent, natural, suspended)

---

## Issue: Composition feels off

**Problem:** Framing doesn't achieve intended visual impact

**Solutions:**
1. Reference composition framework by name (Rule of Thirds, Golden Ratio)
2. Specify negative space percentage (70% empty)
3. Describe subject position explicitly (center, right-third, lower-left)
4. Include frame-within-frame elements if desired
5. Mention leading lines, diagonals, or symmetry explicitly

---

## Issue: Style preset conflicts with base

**Problem:** Applying style creates contradictions in prompt

**Solutions:**
1. Check compatibility notes in preset (what it works/conflicts with)
2. Modify preset elements to match base requirements
3. Apply preset selectively (color only, lighting only, post only)
4. Create hybrid by blending compatible elements from multiple presets
5. Prioritize base template technical requirements over style aesthetics

---

# ADVANCED TECHNIQUES

## Technique 1: Hybrid Style Mixing

**Concept:** Combine elements from multiple style presets

**Example:** Blade Runner aesthetic = Cyberpunk + Film Noir
```
- Cyberpunk: Neon colors, rain, urban night
- Film Noir: High contrast, low angles, mystery
- Result: Neon noir, wet streets, dramatic shadows with colored light
```

**Application:**
1. Choose primary preset (dominant aesthetic)
2. Select compatible elements from secondary preset
3. Resolve conflicts by prioritizing primary
4. Test color palette compatibility first (most common conflict)

---

## Technique 2: Modular Component Stacking

**Concept:** Layer multiple components from same category for complexity

**Example:** Complex camera movement
```
- DOLLY-01 Slow Push-In (8 inches forward)
- + CRANE-01 Rising Reveal (2 feet vertical)
- + PAN-01 Slow Pan (30° right)
- = Compound diagonal movement revealing environment while approaching
```

**Application:**
1. Start with primary movement (most important)
2. Add compatible secondary movement
3. Specify coordination (simultaneous or sequential)
4. Keep total to 2-3 max (more creates confusion)

---

## Technique 3: Beat-Synchronized Action

**Concept:** Choreograph multiple elements to same beat structure

**Example:** Product reveal synchronized
```
Beat 0.0s: Product in shadow, camera static, music note
Beat 2.0s: Light begins revealing, camera push begins, music builds
Beat 4.0s: Product fully lit, camera close, music peak
Beat 6.0s: Product rotation begins, camera locks, music sustains
```

**Application:**
1. Establish beat structure first (timing framework)
2. Assign each element (light, camera, subject) to beats
3. Synchronize key moments (reveals, peaks, transitions)
4. Include timing in prompt explicitly

---

## Technique 4: Negative Prompting Precision

**Concept:** Use AVOID section strategically to eliminate unwanted elements

**Example:**
```
AVOID: Smooth gimbal movement, warm color temperature, saturated colors,
modern LED characteristics, clean digital look, beauty lighting, smile,
optimistic mood, daylight, symmetrical composition

Each "avoid" actively pushes generation away from unwanted aesthetic
```

**Application:**
1. List specific opposite of desired aesthetic
2. Include technical opposites (smooth vs handheld, warm vs cool)
3. Mention aesthetic traps for your content type
4. Keep avoid list focused (5-10 items maximum)

---

## Technique 5: Reference Blending

**Concept:** Reference real-world examples within prompt

**Example:**
```
"Color grade: Reference David Fincher's 'Zodiac' color science - teal
shadows, desaturated -25%, lifted blacks creating slight flat feel"

"Lighting: Reference Caravaggio chiaroscuro - single hard source creating
dramatic religious painting quality"
```

**Application:**
1. Reference cinematographers, directors, painters for visual style
2. Reference specific films/artworks (Blade Runner, Rembrandt portraits)
3. Keep references specific not general ("Fincher" not "thriller movies")
4. Use references to supplement technical specs, not replace

---

## Technique 6: Environmental Storytelling

**Concept:** Use environmental details to suggest narrative without explicit story

**Example:**
```
"Coffee cup half-empty, ring stain on desk, overflowing ashtray, desk lamp
on despite daylight visible through window suggesting all-night work session,
scattered photographs, red string connecting images on cork board, detective
case obsession visible through environmental accumulation"
```

**Application:**
1. Add specific objects suggesting use/time/purpose
2. Include wear patterns (dust, stains, damage)
3. Layer temporal clues (old + new items, accumulation)
4. Suggest human presence through object arrangement

---

# DEADMAN BROADCAST INTEGRATION

## Using DEADMAN Templates with This Library

**DEADMAN Aesthetic = Analog Horror Preset + Specific Modular Components**

### Core DEADMAN Formula:

```
BASE: Documentary or Environment templates
+ COMPONENTS:
  - VHS 1987 technical degradation
  - Practical-only lighting (CRT, ON AIR, fluorescent)
  - Static surveillance or handheld nervous camera
  - Institutional horror color palette
  - 60Hz hum + analog audio
+ STYLE: Analog Horror Preset
= DEADMAN BROADCAST aesthetic
```

### Quick DEADMAN Prompt Builder:

**Step 1:** Choose DEADMAN scenario type:
- Broadcast console (authority/control)
- Surveillance feed (observation/paranoia)
- Abandoned office (institutional horror)
- CRT monitor focus (data/technology)
- Underground studio (bunker/isolation)

**Step 2:** Add DEADMAN-specific components:
```
VHS LAYER:
- VHS recording 1987, 480i resolution
- Horizontal scanlines 2px spacing
- Tracking errors, chroma noise
- Timestamp overlay VCR font

LIGHTING LAYER:
- Practical only (no film lights)
- CRT phosphor green #33FF33
- ON AIR tally red #FF2020, 2Hz flicker
- Fluorescent 4100K institutional
- 20:1+ extreme contrast

COLOR LAYER:
- Desaturate -30% global
- Tech colors 100-120% (red, green, cyan)
- Void black #0A0A0A dominant
- Institutional green tint

AUDIO LAYER:
- 60Hz electrical hum -40dB
- Analog static -50dB
- CRT electron hum (if monitors present)
- Mechanical relay clicks
- HPF 80Hz / LPF 12kHz
```

**Step 3:** Combine with situation:
```
[DEADMAN BASE SITUATION]
+ VHS technical characteristics
+ Practical lighting only
+ DEADMAN color palette
+ Analog audio specification
= Production-ready DEADMAN prompt
```

### Example DEADMAN Integration:

**Scenario:** Corporate whistleblower documentary reveal

**Using This Library:**
1. Base: DOC-02 Interview Subject (for structure)
2. Modify lighting to: SPEC-01 Practical-Only Ambient
3. Add: Analog Horror Preset (complete DEADMAN aesthetic)
4. Customize: Subject = anonymous source, Environment = underground broadcast

**Result:**
```
VHS recording 1987, 480i resolution, visible horizontal scanlines 2px
spacing, tracking errors, chroma noise. Photorealistic interview of
anonymous corporate whistleblower (silhouette only) in underground broadcast
bunker. Subject backlit by single CRT monitor displaying green phosphor
#33FF33 scrolling data creating silhouette. Red ON AIR tally light #FF2020
flickers 2Hz camera-right.

Shot on consumer VHS camcorder simulated, 480i interlaced. Static locked
surveillance angle 8ft height. Autofocus occasionally hunts (VHS
characteristic).

LIGHTING: 100% practical sources only - CRT monitor backlight creating
silhouette, ON AIR tally providing red accent, overhead fluorescent 4100K
creating institutional green tint. 25:1+ extreme contrast, deep void blacks
#0A0A0A.

ENVIRONMENT: Underground broadcast bunker, concrete walls, exposed cables,
vintage 1987 broadcast equipment visible (tape decks, mixing board), cold
55°F temperature implied, dust on equipment showing abandonment.

COLOR: DEADMAN palette - Desaturate -30% global, phosphor green #33FF33 at
100%, signal red #FF2020 at 120%, void black #0A0A0A dominant, institutional
green cast overall.

VHS DEGRADATION: Tracking errors 2-3 times creating horizontal tears, chroma
separation, timestamp "03/15/1987 02:34 AM" white VCR font lower-right,
generation loss artifacts.

AUDIO: 60Hz electrical hum -40dB continuous, analog static -50dB, CRT
electron hum -35dB, voice processed through vintage microphone compression,
HPF 80Hz / LPF 12kHz analog bandwidth limit.

SUBJECT: Anonymous whistleblower silhouette only (identity protection), sits
rigid, occasional nervous hand gestures visible in silhouette, voice altered
(pitch shifted down 3 semitones).

Duration: 10 seconds.

AVOID: Modern digital, warm lighting, beauty aesthetic, smooth camera,
saturated colors, optimism, visible faces.
```

---

# OPTIMIZATION TIPS

## Tip 1: Prompt Length Optimization

**Goal:** Maximum detail in minimum words

**Technique:**
- Use industry terms (fewer words, more meaning)
  - Instead of: "The light is very soft and wraps around the subject"
  - Use: "Wrap-around soft key, 3:1 contrast"

- Combine related specs
  - Instead of: "Shot on RED camera. 4K resolution. 24 frames per second."
  - Use: "Shot on RED V-Raptor, 4K, 24fps."

- Use hex codes vs descriptions
  - Instead of: "Bright vibrant magenta pink color"
  - Use: "Magenta #FF00FF"

**Target:** 200-350 words for detailed prompt, 150-200 for simple

---

## Tip 2: Hierarchical Detail

**Concept:** Most important details first, refinements later

**Structure:**
```
1. CORE CONCEPT (subject + environment + mood) - 1 sentence
2. CAMERA SPECS (camera, lens, movement) - 1-2 sentences
3. LIGHTING (setup, contrast, color temp) - 2-3 sentences
4. COMPOSITION (framing, rule, elements) - 1-2 sentences
5. COLOR (palette, grading, specific codes) - 1-2 sentences
6. DETAILS (textures, atmosphere, specifics) - 2-4 sentences
7. POST (grading, effects, duration) - 1-2 sentences
8. AVOID (negative constraints) - 1 sentence
```

**Benefit:** If Sora 2 truncates, most critical info processed first

---

## Tip 3: Consistency Tokens

**Concept:** Repeat key terms to reinforce critical elements

**Example:**
```
"Cyberpunk neon aesthetic... neon signs creating... oversaturated neon
+40%... neon reflections in wet streets... background neon bokeh..."

Repeating "neon" throughout reinforces this as core aesthetic element
```

**Application:**
- Identify 3-5 core aesthetic keywords
- Use naturally throughout prompt (not forced)
- Reinforces critical elements to AI

---

## Tip 4: Technical Spec Clustering

**Concept:** Group all technical specs together for clarity

**Format:**
```
TECHNICAL SPECIFICATIONS:
Shot on [CAMERA], [RESOLUTION], [FRAME RATE]
[FOCAL LENGTH] at f/[APERTURE]
[MOVEMENT TYPE] at [SPEED]
Duration: [X] seconds

Keeps all tech specs in one scannable block
```

---

## Tip 5: Testing Workflow

**Process for refining prompts:**

1. Generate 3-5 variations with same prompt (test consistency)
2. Identify common issues across variations
3. Add specificity to problem areas
4. Regenerate with refined prompt
5. Compare new vs old results
6. Iterate until 80%+ satisfaction

**Key:** Don't expect perfection on first generation

---

## Tip 6: Library Combination Shortcuts

**Speed up prompt building:**

Create personal "favorite combinations" file:
```
COMBO A: Cinematic Portrait
- Base: CIN-02
- Movement: DOLLY-01 Slow Push-In
- Lighting: STUDIO-02 Rembrandt
- Color: Teal-Orange grade
- Style: Modern Commercial

COMBO B: Documentary Street
- Base: DOC-04
- Movement: HANDHELD-02 Active Vérité
- Lighting: Available only
- Color: Desaturated -30%
- Style: Gritty Realism

etc.
```

**Benefit:** Copy entire combo, customize specifics only

---

**END OF USAGE GUIDE**

*This comprehensive system provides everything needed to generate production-
quality Sora 2 prompts. Start with Quick Start Workflow, reference libraries
as needed, study examples for inspiration, and iterate toward perfection.*

*The system is modular - use complete or extract pieces. Every component is
production-tested and ready to deploy.*
