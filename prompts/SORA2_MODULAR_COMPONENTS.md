# SORA 2: MODULAR COMPONENT LIBRARY
## Mix-and-Match Building Blocks for Prompt Construction

**Version**: 1.0
**Classification**: COMPONENT REFERENCE
**Purpose**: Reusable components that can be combined with any base template
**Usage**: Copy components and insert into template prompts

---

# TABLE OF CONTENTS

1. [Camera Movement Library](#camera-movement-library)
2. [Lighting Setup Library](#lighting-setup-library)
3. [Motion Descriptor Library](#motion-descriptor-library)
4. [Composition Framework Library](#composition-framework-library)
5. [Atmosphere & Weather Library](#atmosphere-weather-library)
6. [Color Palette Library](#color-palette-library)
7. [Texture & Material Library](#texture-material-library)
8. [Time & Speed Control Library](#time-speed-control-library)

---

# CAMERA MOVEMENT LIBRARY

## Static & Minimal Movement

### LOCKED-01: Absolute Static
```
Camera locked on tripod, zero movement, absolute stability. Frame remains
perfectly static throughout duration allowing subject motion to dominate.
Industrial tripod with sandbags, no breathing room, no drift.
```
**Best For**: Product showcases, interviews, technical documentation
**Avoid With**: Long durations (static fatigue), action sequences

---

### LOCKED-02: Breathing Room
```
Camera on tripod with imperceptible organic drift. Subtle 2-3mm movement
over duration suggests handheld humanity without distraction. Natural
settling, not mechanical precision.
```
**Best For**: Intimate moments, contemplative scenes, documentary realism
**Avoid With**: Product work requiring perfect stability

---

### LOCKED-03: Motivated Reframe
```
Camera begins locked, executes single deliberate reframe at [X]-second mark,
locks again. Movement motivated by subject action or reveal. Smooth 1-second
transition between compositions.
```
**Best For**: Reveals, reaction shots, following subject repositioning
**Avoid With**: Continuous action requiring constant tracking

---

## Linear Movement (Dolly/Track/Slider)

### DOLLY-01: Slow Push-In
```
Camera dolly forward on track [X] inches over [Y] seconds at constant [Z]
ft/sec. Smooth engagement with subject, increasing intimacy. Steadicam or
motorized slider for vibration-free movement.
```
**Speeds**:
- 0.3 ft/sec = Subliminal, barely perceptible
- 0.5 ft/sec = Contemplative, gentle
- 1.0 ft/sec = Standard narrative
- 2.0 ft/sec = Purposeful, deliberate
- 3.0 ft/sec = Urgent, motivated

**Example**: `Camera slow dolly forward 8 inches over 10 seconds (0.66 ft/sec),
imperceptible engagement, Steadicam smooth.`

---

### DOLLY-02: Pull-Back Reveal
```
Camera dolly backward on track [X] feet over [Y] seconds revealing
[CONTEXT/SCALE/ENVIRONMENT]. Begins close on [DETAIL], expands to show
[WIDER CONTEXT]. Creates "oh, that's where we are" moment.
```
**Best For**: Environmental reveals, scope demonstrations, context establishment
**Avoid With**: Maintaining intimacy, close emotional moments

**Example**: `Camera pulls back 3 feet over 8 seconds revealing subject is
alone in vast empty warehouse. Begins extreme close-up on face, ends wide
shot showing isolation.`

---

### DOLLY-03: Lateral Tracking (Truck)
```
Camera trucks laterally [LEFT/RIGHT] on track parallel to subject at [SPEED].
Maintains consistent subject distance while environment passes in background
creating parallax depth. Reveals subject from multiple angles during single
shot.
```
**Best For**: Walking subjects, product reveals, dynamic environments
**Avoid With**: Static subjects where movement creates confusion

**Example**: `Camera trucks left 6 feet over 12 seconds parallel to walking
figure, maintaining 8-foot subject distance. Background architecture creates
parallax depth.`

---

### DOLLY-04: Compound Movement (Dolly + Boom)
```
Camera combines dolly [DIRECTION] with simultaneous boom [UP/DOWN] creating
diagonal path through space. Adds production value and spatial complexity.
[X] feet horizontal, [Y] feet vertical over [Z] seconds.
```
**Best For**: High-end cinematics, establishing shots, spatial reveals
**Avoid With**: Simple scenes not requiring complexity

**Example**: `Camera dolly forward 4 feet while boom up 2 feet over 10
seconds. Creates ascending reveal of location while approaching subject.`

---

## Rotation (Pan/Tilt)

### PAN-01: Slow Pan Reveal
```
Camera rotates horizontally [LEFT/RIGHT] [X] degrees over [Y] seconds on
tripod head. Smooth constant velocity revealing [ENVIRONMENT/NEW ELEMENT].
Fluid head resistance set to [LIGHT/MEDIUM/HEAVY] drag.
```
**Degrees/Timing**:
- 30° = Subtle reframe
- 90° = Quarter turn, significant reveal
- 180° = Half rotation, complete perspective shift
- 360° = Full rotation, environmental survey

**Example**: `Camera slow pan right 90 degrees over 8 seconds revealing
abandoned room. Medium drag creating smooth constant rotation.`

---

### TILT-01: Vertical Reveal
```
Camera tilts vertically [UP/DOWN] [X] degrees over [Y] seconds. Begins on
[STARTING ELEMENT], tilts to reveal [ENDING ELEMENT]. Emphasizes scale,
height, or vertical relationship.
```
**Best For**: Architecture, scale reveals, sky-to-ground transitions
**Avoid With**: Horizontal compositions where vertical movement confuses

**Example**: `Camera tilts up 60 degrees over 6 seconds. Begins on feet,
rises to reveal towering skyscraper above.`

---

### PAN-02: Whip Pan Transition
```
Camera executes rapid pan blur [LEFT/RIGHT] over [0.3-0.8] seconds creating
motion blur transition effect. Speed [MODERATE/EXTREME] based on desired
blur intensity. Used as cut alternative or energy punctuation.
```
**Best For**: Transitions, high-energy moments, style punctuation
**Avoid With**: Serious documentary, formal content, vertigo-sensitive viewers

**Example**: `Camera whip pans right 180 degrees over 0.4 seconds creating
complete motion blur. Extreme speed transition to new scene.`

---

## Handheld & Operated Movement

### HANDHELD-01: Documentary Subtle
```
Camera handheld shoulder-mounted with subtle organic shake. Natural operator
breathing and weight shifts visible but minimal (1-3mm displacement). Film-
style documentary authenticity without distraction.
```
**Best For**: Documentary, realism, intimate moments, run-and-gun
**Avoid With**: Formal product work, technical showcases

**Example**: `Camera handheld shoulder-mount, documentary subtle shake,
natural breathing rhythm visible creating authentic observation feel.`

---

### HANDHELD-02: Active Vérité
```
Camera handheld with active operator movement following subject through
environment. Reactive not predictive - follows action as it unfolds. Organic
frame adjustments, occasional soft focus during rapid reframes, authentic
mistakes preserved.
```
**Best For**: Action following, breaking news feel, sports coverage, chaos
**Avoid With**: Composed formal scenes, product beauty shots

**Example**: `Camera active handheld following subject through crowded
market. Reactive movements, slight frame corrections visible, occasional
soft focus during fast pans creating documentary immediacy.`

---

### HANDHELD-03: Steadicam Float
```
Camera on Steadicam rig creating floating smooth movement with subtle organic
imperfection. Not gimbal-perfect, retains slight human quality. Operator
walks at [PACE] creating [SMOOTH/SLIGHTLY IRREGULAR] movement.
```
**Best For**: Following subjects, immersive tracking, single-take sequences
**Avoid With**: Perfect stability requirements, static locked compositions

**Example**: `Camera Steadicam float following subject through hallway at
walking pace. Smooth but retains subtle operator presence, organic height
variation from footsteps.`

---

### HANDHELD-04: Chaotic Energy
```
Camera aggressive handheld with pronounced movement. High energy shake,
rapid reframes, dynamic instability suggesting chaos, urgency, or POV
distress. 10-20mm displacement, fast reframe corrections.
```
**Best For**: Horror POV, action chaos, found footage, panic scenes
**Avoid With**: Any scene requiring composure or clarity

**Example**: `Camera chaotic handheld, aggressive shake suggesting panic,
rapid uncontrolled reframes, high energy instability creating distress POV.`

---

## Aerial & Crane Movement

### AERIAL-01: Drone Ascent
```
Camera autonomous drone ascent [X] feet over [Y] seconds revealing
environmental scale. Begins [LOW/GROUND LEVEL], rises to [ELEVATED
PERSPECTIVE]. Smooth automated movement, perfectly stabilized.
```
**Best For**: Establishing shots, scale reveals, location introductions
**Avoid With**: Intimate moments, close detail work

**Example**: `Drone slow ascent 60 feet over 12 seconds. Begins ground
level, rises revealing full scope of landscape. Smooth autonomous flight.`

---

### AERIAL-02: Orbital Circle
```
Camera drone executes circular orbit around [SUBJECT] at [RADIUS] maintaining
constant altitude and speed. [CLOCKWISE/COUNTER-CLOCKWISE] rotation over
[DURATION] creating 360° reveal while subject remains centered.
```
**Best For**: Subject showcases, environmental context, dynamic reveals
**Avoid With**: Fast-moving subjects, tight indoor spaces

**Example**: `Drone orbital at 50-foot radius around lighthouse,
counter-clockwise 360° rotation over 20 seconds. Subject centered,
environment reveals.`

---

### CRANE-01: Rising Reveal
```
Camera crane up [X] feet over [Y] seconds while [MAINTAINING SUBJECT FRAMING/
REVEALING ENVIRONMENT]. Begins [LOW ANGLE], rises to [HIGH PERSPECTIVE].
Jib arm smooth automated movement.
```
**Best For**: Dramatic reveals, environmental scope, opening/closing shots
**Avoid With**: Intimate close-ups, minimal production environments

**Example**: `Camera crane up 12 feet over 10 seconds rising from eye-level
intimate portrait to high angle revealing subject's environmental context.`

---

## Advanced & Specialized Movement

### DOLLY-ZOOM-01: Vertigo Effect
```
Camera dolly [FORWARD/BACKWARD] while simultaneously zoom [OPPOSITE
DIRECTION] maintaining subject size while background perspective warps.
Creates disorientation, unease, realization effect. Precise coordination
required.
```
**Best For**: Psychological moments, realizations, horror, disorientation
**Avoid With**: Naturalistic scenes, documentary realism

**Example**: `Camera dolly back 4 feet while zoom in from 35mm to 70mm over
3 seconds. Subject size constant, background compresses creating vertigo
unease.`

---

### GIMBAL-01: Impossible Stabilization
```
Camera on 3-axis gimbal creating impossibly smooth movement through
[TERRAIN/OBSTACLES]. Perfect stabilization during [RUNNING/STAIRS/ROUGH
GROUND]. Modern tech-perfect aesthetic, not organic.
```
**Best For**: Action following, modern commercial look, tech showcases
**Avoid With**: Period pieces, documentary authenticity, organic realism

**Example**: `Camera gimbal-stabilized following parkour subject running
over obstacles. Perfectly smooth despite operator running, impossibly stable
modern aesthetic.`

---

### MOTION-CONTROL-01: Precise Repeatability
```
Camera on motion control rig executing programmed movement with [SUB-
MILLIMETER] precision. Identical movement repeatable for VFX plates or
multiple takes. Automated [SPEED] over [PATH].
```
**Best For**: VFX work, product showcases, precision requirements
**Avoid With**: Documentary, spontaneous moments, organic scenes

**Example**: `Motion control rig executes programmed 8-second arc around
product with 0.1mm precision. Repeatable for multiple lighting passes.`

---

# LIGHTING SETUP LIBRARY

## Natural Light Setups

### NAT-01: Golden Hour Backlight
```
Natural sunlight 0-30 minutes [AFTER SUNRISE/BEFORE SUNSET] positioned
behind subject creating rim light and warm 3200-3800K glow. Soft diffused
fill from open sky at -2 stops. Subject backlit creating separation and
warmth. Lens flare acceptable if motivated.
```
**Color Temperature**: 3200-3800K (warm orange)
**Contrast**: 6:1 to 10:1
**Best For**: Romantic, nostalgic, beauty, dreamy aesthetics
**Time Window**: 30-minute maximum capture window

**Example**: `Golden hour backlight 20 minutes before sunset, subject
silhouetted with warm rim light, soft sky fill, acceptable motivated lens
flare, 3600K warmth creating nostalgic mood.`

---

### NAT-02: Overcast Soft
```
Overcast cloud cover creating massive natural softbox. Even diffused light
from entire sky dome, shadowless illumination. Neutral 6500K color
temperature. Low contrast 3:1, flattering for skin tones, eliminating harsh
shadows.
```
**Color Temperature**: 6000-6500K (neutral)
**Contrast**: 2:1 to 4:1 (very low)
**Best For**: Portraits, product, commercial beauty, even illumination
**Weather Required**: Complete overcast, no sun breaks

**Example**: `Overcast sky creating natural softbox, shadowless even
illumination, 6500K neutral, 3:1 contrast perfect for portrait skin tones.`

---

### NAT-03: North Window (Indirect)
```
Large north-facing window (northern hemisphere) providing indirect daylight.
Soft directional light 5000-5500K, no direct sun. Creates gentle modeling
with soft shadows. White bounce card opposite window for fill at -1.5 stops.
```
**Color Temperature**: 5000-5500K (neutral-cool)
**Contrast**: 4:1 to 6:1
**Best For**: Interviews, portraits, product, natural indoor looks
**Setup**: Subject 4-6 feet from window, bounce opposite

**Example**: `North window indirect daylight as key, soft directional
modeling, white bounce fill opposite at -1.5 stops, 5200K natural indoor
quality.`

---

### NAT-04: Direct Sun Hard Light
```
Direct midday sun creating harsh key light with hard-edged shadows. High
contrast 16:1+, dramatic modeling. 5200-5600K neutral daylight. No fill or
minimal fill creating noir-like drama. Embrace harsh aesthetic.
```
**Color Temperature**: 5200-5600K (neutral)
**Contrast**: 12:1 to 20:1 (very high)
**Best For**: Drama, noir, harsh realism, sculptural subjects
**Challenges**: Harsh shadows, squinting subjects, high dynamic range

**Example**: `Harsh midday sun direct overhead creating hard dramatic
shadows, 5400K neutral, 16:1 contrast, no fill allowing deep blacks, noir
aesthetic.`

---

### NAT-05: Blue Hour Twilight
```
Natural light 30-60 minutes [BEFORE SUNRISE/AFTER SUNSET] creating deep blue
ambient 7500-9000K. Very low light level requiring high ISO or long exposure.
Cool ethereal mood, minimal contrast 3:1. Practical lights appear warm by
comparison.
```
**Color Temperature**: 7500-9000K (cool blue)
**Contrast**: 2:1 to 4:1 (low, ambient)
**Best For**: Mood, atmosphere, twilight magic, practical light showcases
**Challenges**: Low light levels, narrow time window

**Example**: `Blue hour 45 minutes after sunset, deep blue 8200K ambient,
low contrast 3:1, practical building lights appear warm gold by comparison.`

---

## Studio Lighting Setups (Artificial)

### STUDIO-01: Three-Point Classic
```
Standard three-point lighting setup. Key light camera-left 45° at subject
height, 5600K LED panel. Fill light camera-right 45° at -2 stops. Rim/back
light elevated behind subject opposite key creating edge separation. 6:1
contrast ratio.
```
**Lights Required**: 3 (Key, Fill, Rim)
**Contrast**: 4:1 to 8:1 (adjustable via fill)
**Best For**: Interviews, standard portraits, product, commercial
**Color Temperature**: Matched 5600K daylight balanced

**Example**: `Three-point classic: Key camera-left 45° at subject height
creating modeling, fill camera-right -2 stops, elevated rim backlight for
separation, 6:1 contrast.`

---

### STUDIO-02: Rembrandt Portrait
```
Single key light positioned 45° above and 45° to side of subject creating
triangular highlight on shadow-side cheek (Rembrandt triangle). No fill or
minimal fill. 8:1 to 12:1 contrast. Dramatic portrait lighting emphasizing
facial structure.
```
**Lights Required**: 1-2 (Key, optional minimal fill)
**Contrast**: 8:1 to 16:1 (high drama)
**Best For**: Character portraits, dramatic imagery, classical painting look
**Setup**: Key at 45°/45° until triangle appears on cheek opposite light

**Example**: `Rembrandt lighting: Single key 45° up and 45° camera-left
creating triangle on right cheek, minimal fill, 12:1 contrast, dramatic
classical portrait.`

---

### STUDIO-03: Butterfly/Paramount
```
Single large soft key light directly in front of subject elevated 30-40°
creating symmetrical butterfly-shaped shadow under nose. Fill from below via
reflector. Glamour lighting flattening facial features, hiding texture.
Hollywood golden age aesthetic.
```
**Lights Required**: 1-2 (Overhead key, reflector fill)
**Contrast**: 3:1 to 5:1 (glamour softness)
**Best For**: Beauty, glamour, fashion, classic Hollywood portraits
**Setup**: Large softbox centered above subject angled down 30-40°

**Example**: `Butterfly glamour lighting: Large softbox overhead centered
creating symmetrical nose shadow, white reflector fill below, 4:1 soft
contrast hiding texture.`

---

### STUDIO-04: Edge/Rim Only
```
Subject lit only from behind/sides with rim lights creating edge definition
against dark background. No frontal key light. Subject appears as silhouette
with glowing edges. High drama 20:1+ contrast. Mystery, concealment, graphic
impact.
```
**Lights Required**: 2-4 (Edge/rim lights only)
**Contrast**: 20:1+ (extreme)
**Best For**: Silhouettes, mystery, drama, graphic compositions
**Setup**: Lights behind subject aimed at edges, no front light

**Example**: `Edge light only setup: Two rim lights behind subject creating
glowing outline, no frontal key, silhouette with defined edges, 20:1+
contrast mystery mood.`

---

### STUDIO-05: High-Key Commercial
```
Bright even illumination minimizing shadows. Multiple large soft sources
creating wrap-around light. White or light background. Low contrast 2:1 to
3:1. Clean commercial aesthetic, optimistic mood, maximum visibility of
product/subject.
```
**Lights Required**: 4+ (Multiple soft sources, background lights)
**Contrast**: 2:1 to 3:1 (very low)
**Best For**: Product, commercial, corporate, optimistic advertising
**Setup**: Soft sources from multiple angles, overlit for flatness

**Example**: `High-key commercial: Four large soft LED panels from cardinal
directions, white background separately lit, 2:1 flat contrast, bright clean
optimistic aesthetic.`

---

### STUDIO-06: Low-Key Noir
```
Single hard source creating dramatic shadows and limited illumination.
Subject partially lit, deep blacks dominate frame. 16:1 to 25:1 contrast.
Film noir aesthetic, mystery, drama, selective revelation. Embrace darkness.
```
**Lights Required**: 1 (Single hard key)
**Contrast**: 16:1 to 25:1+ (extreme)
**Best For**: Noir, mystery, drama, thriller, selective emphasis
**Setup**: Single hard fresnel or open-face creating directional hard light

**Example**: `Low-key noir: Single hard fresnel from camera-left creating
dramatic shadows, no fill, deep blacks dominate, 20:1 contrast, mystery
through selective revelation.`

---

## Specialized & Practical Lighting

### SPEC-01: Practical-Only Ambient
```
100% in-scene practical light sources only. No added film lights. Lamps,
candles, windows, neon, screens provide all illumination. Motivated realism,
natural falloff, authentic light behavior. Accept mixed color temperatures
and high contrast.
```
**Lights Required**: 0 film lights (practicals only)
**Contrast**: Variable (uncontrolled by practicals)
**Best For**: Naturalism, realism, ambient authenticity, night interiors
**Challenges**: Exposure control, mixed color temperature, limited output

**Example**: `Practical-only lighting: Room lit solely by desk lamp (3200K),
window moonlight (8000K), computer screen (6500K). Mixed color temps,
natural falloff, authentic ambient.`

---

### SPEC-02: Volumetric Fog/Haze
```
Atmospheric haze or fog introduced creating visible light beams. Single or
multiple hard sources penetrating atmosphere creating volumetric god rays.
Particles scatter light making beams visible. Adds depth and drama.
```
**Equipment Required**: Fog/haze machine + hard light sources
**Best For**: Atmosphere, drama, depth, visual interest, night scenes
**Density**: Light haze (subtle beams) to heavy fog (dense atmosphere)

**Example**: `Volumetric fog setup: Atmospheric haze throughout space,
single hard fresnel from window position creating visible beam through fog,
god ray effect, dramatic depth.`

---

### SPEC-03: Motivated Neon/Colored Practical
```
Colored practical lights (neon signs, LED strips, colored bulbs) providing
motivated color accents. Practical sources visible in frame justifying color.
Mixed color temperatures creating visual interest. Cyberpunk, urban night,
club aesthetics.
```
**Color**: Multiple (magenta, cyan, amber, green typical)
**Best For**: Night scenes, urban environments, cyberpunk, music venues
**Setup**: Visible neon/LED practicals providing motivation for colored light

**Example**: `Motivated neon: Visible magenta neon sign in frame providing
motivated magenta key light on subject, cyan LED strip as rim, mixed color
temperature urban aesthetic.`

---

### SPEC-04: Fire/Flame Practical
```
Real fire (candles, fireplace, torch) or fire simulation providing warm
flickering motivated light. 2200-2700K very warm. Organic flicker pattern
(2-5Hz irregular). Intimate, primitive, or medieval atmospheres.
```
**Color Temperature**: 2200-2700K (very warm orange)
**Flicker**: 2-5Hz irregular organic pattern
**Best For**: Period pieces, intimate moments, primitive settings, romance
**Safety**: Real fire requires safety protocols

**Example**: `Fireplace practical: Real fire providing warm 2400K flickering
key light, organic flame movement reflected in faces, primitive intimate
atmosphere, safety crew on standby.`

---

### SPEC-05: Single Candle Darkness
```
Extreme low-key lighting using single candle as only light source. Very warm
2200K, minimal output requiring high ISO. Intimate scale, extreme contrast
20:1+, faces partially lit. Baroque painting aesthetic, extreme intimacy or
period authenticity.
```
**Color Temperature**: 2000-2200K (very warm)
**Contrast**: 20:1+ (extreme)
**Best For**: Period pieces, extreme intimacy, Baroque painting aesthetics
**Challenges**: Very low light, high noise, limited illumination radius

**Example**: `Single candle lighting: One candle providing all illumination,
very warm 2100K, faces partially lit with deep shadows, 25:1 contrast,
Baroque painting aesthetic.`

---

# MOTION DESCRIPTOR LIBRARY

## Subject Movement Descriptors

### MOTION-SUBJ-01: Slow Deliberate
```
Subject moves at [0.5-1.0 ft/sec], each movement intentional and controlled.
Pace suggests thoughtfulness, care, precision, or ceremonial purpose.
Movements complete fully before next begins. Contemplative rhythm.
```
**Emotional Weight**: Thoughtful, careful, ceremonial, weighted
**Best For**: Craftsmanship, ritual, precision work, emotional moments
**Example**: `Subject's hands move slowly and deliberately, 0.7 ft/sec,
completing each gesture fully before next, suggesting ritual importance.`

---

### MOTION-SUBJ-02: Natural Conversational
```
Subject moves at normal human pace [1.5-2.5 ft/sec], gestures and actions
flow naturally. Realistic timing, authentic rhythm, no performance quality.
Documentary naturalism, unaware of camera, life-speed.
```
**Emotional Weight**: Neutral, realistic, authentic, unperformed
**Best For**: Documentary, realism, dialogue scenes, authentic behavior
**Example**: `Subject natural conversational movement, 2.0 ft/sec average,
gestures flow organically, no performance awareness, documentary authentic.`

---

### MOTION-SUBJ-03: Energetic/Urgent
```
Subject moves rapidly [3-5 ft/sec], quick decisive actions suggesting urgency,
excitement, or energy. Movements overlap, minimal pause between actions.
High tempo creates tension or dynamism.
```
**Emotional Weight**: Urgent, excited, energetic, tense
**Best For**: Action, urgency, high-energy moments, pursuit
**Example**: `Subject rapid movements 4 ft/sec, actions overlapping, minimal
pauses, creating urgent energetic rhythm suggesting time pressure.`

---

### MOTION-SUBJ-04: Hesitant/Uncertain
```
Subject movement includes pauses, false starts, micro-retreats. Speed varies
[0.3-1.5 ft/sec], rhythm irregular. Suggests uncertainty, fear, reluctance,
or internal conflict. Movement fights against itself.
```
**Emotional Weight**: Uncertain, fearful, reluctant, conflicted
**Best For**: Suspense, internal struggle, fear, difficult decisions
**Example**: `Subject hesitant movement, reaches toward object then pauses,
slight retreat, irregular rhythm 0.8 ft/sec average, suggesting fear and
internal conflict.`

---

### MOTION-SUBJ-05: Exhausted/Weighted
```
Subject movements slower than natural [0.8-1.5 ft/sec] with visible effort.
Slight sag, weight visible in posture, movements require recovery pauses.
Suggests physical exhaustion, emotional weight, or burden.
```
**Emotional Weight**: Exhausted, burdened, defeated, heavy
**Best For**: Fatigue scenes, emotional weight, physical struggle
**Example**: `Subject exhausted movement, 1.0 ft/sec with visible effort,
slight sag in shoulders, pauses for recovery between actions, weight of
exhaustion visible.`

---

## Camera-to-Subject Relationship Motion

### MOTION-REL-01: Approach/Engagement
```
Camera moves toward subject decreasing distance from [X to Y feet] over
[duration]. Creates increasing intimacy, engagement, focus. Viewer drawn
into subject's space. Speed determines gentleness vs. urgency of engagement.
```
**Psychological Effect**: Increasing intimacy, focus, engagement
**Best For**: Reveals, engagement moments, drawing viewer in
**Example**: `Camera slow approach from 12 feet to 4 feet over 8 seconds,
gentle engagement increasing intimacy with subject, contemplative pace.`

---

### MOTION-REL-02: Retreat/Revelation
```
Camera moves away from subject increasing distance from [X to Y feet] over
[duration]. Reveals context, scale, or isolation. Viewer pulled back to
observe. Creates "oh, now I understand" moment through expanded perspective.
```
**Psychological Effect**: Context reveal, scale demonstration, isolation
**Best For**: Environmental reveals, scale demonstrations, "big picture"
**Example**: `Camera retreat from 3 feet to 15 feet over 10 seconds revealing
subject alone in vast space, isolation emphasized through expanding frame.`

---

### MOTION-REL-03: Parallel Tracking
```
Camera maintains constant distance while moving parallel to moving subject.
Creates sense of accompaniment, observation, or pursuit. Viewer moves with
subject through space. Background parallax reveals depth and movement.
```
**Psychological Effect**: Accompaniment, observation, pursuit
**Best For**: Walking scenes, journey moments, dynamic subjects
**Example**: `Camera tracks parallel to walking subject, maintains 6-foot
distance, background creates parallax depth, viewer accompanies journey.`

---

### MOTION-REL-04: Orbiting Observation
```
Camera circles around static or slow-moving subject maintaining constant
distance. Reveals subject from multiple angles in single shot. Creates
comprehensive observation, showcase moment, or surveillance feeling depending
on speed.
```
**Psychological Effect**: Observation, showcase, surveillance, inspection
**Best For**: Product reveals, character introduction, 360° subject view
**Example**: `Camera orbital around subject at 8-foot radius, 180-degree
arc over 12 seconds, revealing multiple angles, observation perspective.`

---

### MOTION-REL-05: Convergent Paths
```
Camera and subject both move, paths converging to meet or cross. Creates
anticipation of encounter, collision, or intersection. Timing of convergence
determines tension level.
```
**Psychological Effect**: Anticipation, encounter, collision, intersection
**Best For**: Meeting moments, confrontations, path crossings
**Example**: `Camera dolly right while subject walks left, paths converge
at center frame at 6-second mark, encounter moment choreographed.`

---

## Speed Variation Descriptors

### MOTION-SPEED-01: Real-Time Natural
```
Action occurs at actual real-world speed, 100% playback. Natural physics,
authentic timing, documentary realism. 24fps capture, 24fps playback. What
you see is what happened.
```
**Frame Rate**: 24fps capture and playback
**Speed Multiplier**: 1.0x (100%)
**Best For**: Realism, documentary, natural action, dialogue
**Example**: `Real-time natural motion, 24fps capture and playback, 1.0x
speed, authentic physics and timing preserved.`

---

### MOTION-SPEED-02: Subtle Slow-Motion
```
Slightly slower than real-time [60-75% speed]. Captured at 30-48fps,
conformed to 24fps playback. Subtle slowdown adding slight weight and
emphasis without obvious slow-motion. Feels "cinematic" not "slow-mo."
```
**Frame Rate**: 30-48fps capture → 24fps playback
**Speed Multiplier**: 0.6-0.75x (60-75%)
**Best For**: Cinematic feel, subtle emphasis, gentle weight
**Example**: `Subtle slow-motion at 75% speed, shot 32fps conform to 24fps,
gentle cinematic weight without obvious slow-mo.`

---

### MOTION-SPEED-03: Dramatic Slow-Motion
```
Significantly slowed [25-50% speed]. Captured at 60-120fps, conformed to
24fps playback. Obvious slow-motion creating drama, emphasis, or beauty in
motion. Frozen details, suspended moments.
```
**Frame Rate**: 60-120fps capture → 24fps playback
**Speed Multiplier**: 0.25-0.5x (25-50%)
**Best For**: Action moments, impacts, emotional peaks, beauty
**Example**: `Dramatic slow-motion at 40% speed, shot 60fps conform to
24fps, action peak emphasized, details frozen.`

---

### MOTION-SPEED-04: Extreme Slow-Motion
```
Extremely slowed [10-25% speed]. Captured at 120-240fps+, conformed to 24fps
playback. Reveals details invisible to naked eye. Physics visualization,
fluid dynamics, micro-expressions. Scientific or dramatic beauty.
```
**Frame Rate**: 120-240fps+ capture → 24fps playback
**Speed Multiplier**: 0.1-0.25x (10-25%)
**Best For**: Impact details, fluid dynamics, micro-moments, science
**Example**: `Extreme slow-motion at 20% speed, shot 120fps conform to
24fps, reveals water droplet physics invisible to naked eye.`

---

### MOTION-SPEED-05: Time-Lapse Acceleration
```
Significantly accelerated [200-10000% speed]. Clouds rush, sun arcs, crowds
blur. Captures long duration compressed to seconds. Shows passage of time,
natural cycles, or accumulated change.
```
**Frame Rate**: 1 frame per [X seconds] → 24fps playback
**Speed Multiplier**: 200-10000x (varies widely)
**Best For**: Time passage, natural cycles, accumulation, change
**Example**: `Time-lapse at 500x speed, 1 frame every 20 seconds over 2
hours compressed to 15 seconds, sunset accelerated.`

---

### MOTION-SPEED-06: Speed Ramp (Variable)
```
Speed varies during shot transitioning smoothly between [SLOW] and [FAST].
Typical: begins normal, ramps to slow-motion at peak moment, returns to
normal. Requires high frame rate capture (120fps+) with variable conform.
```
**Frame Rate**: 120fps+ capture → variable conform to 24fps
**Speed Multiplier**: Variable (transitions between speeds)
**Best For**: Dramatic emphasis, stylistic moments, impact highlights
**Example**: `Speed ramp from 100% to 30% at impact moment, then return to
100%. Shot 120fps, variable conform creating smooth transition.`

---

# COMPOSITION FRAMEWORK LIBRARY

## Classical Composition Rules

### COMP-01: Rule of Thirds
```
Frame divided into 9 equal parts by two horizontal and two vertical lines.
Subject positioned at intersection points (power points) or along lines.
Creates balanced dynamic composition avoiding centered static feel.
```
**Grid**: 3x3 equal divisions
**Power Points**: 4 intersection points
**Best For**: Landscapes, portraits, general composition, balanced dynamics
**Example**: `Subject positioned at right-third power point, eyes on upper
horizontal line, rule of thirds creating balanced dynamic composition.`

---

### COMP-02: Golden Ratio (Fibonacci)
```
Frame divided using golden ratio (1.618:1) creating spiral or phi grid.
Subject positioned at spiral focal point. More organic than rule of thirds,
found in nature. Creates aesthetic tension and natural eye flow.
```
**Ratio**: 1.618:1 divisions
**Focal Point**: Spiral center or phi grid intersection
**Best For**: Organic subjects, natural scenes, aesthetic perfection
**Example**: `Subject face positioned at golden ratio spiral focal point,
composition follows Fibonacci divisions creating natural aesthetic harmony.`

---

### COMP-03: Centered Symmetry
```
Subject perfectly centered creating formal symmetrical composition. Breaks
rule of thirds intentionally for formal, powerful, or mandala-like effect.
Suggests importance, formality, power, or geometric perfection.
```
**Alignment**: Perfect center vertical and horizontal
**Best For**: Formal portraits, architecture, power, geometric subjects
**Example**: `Subject perfectly centered, symmetrical composition creating
formal power, vertical and horizontal center alignment, mandala-like
formality.`

---

### COMP-04: Frame Within Frame
```
Environmental elements create secondary frame around subject. Doorways,
windows, arches, branches form natural frame. Draws eye to subject, adds
depth, creates layered composition.
```
**Framing Elements**: Architectural or natural elements
**Depth**: Foreground frame, middle subject, background context
**Best For**: Portraits, isolation, depth, layered compositions
**Example**: `Subject framed by doorway arch, creating frame-within-frame,
eye drawn to subject, depth through layered composition.`

---

### COMP-05: Leading Lines
```
Environmental lines (roads, fences, architecture) lead viewer's eye toward
subject. Creates depth, movement, and guided attention. Lines converge at
subject position creating focus.
```
**Line Types**: Roads, fences, architecture, natural formations
**Convergence**: Lines lead to subject
**Best For**: Depth, perspective, guided attention, landscapes
**Example**: `Road leading lines converge at distant subject, creating depth
and guiding eye through composition toward focal point.`

---

### COMP-06: Negative Space
```
Large areas of empty space surrounding small subject. Emphasizes isolation,
scale, minimalism, or contemplation. Subject occupies 10-30% of frame, rest
is negative space.
```
**Subject Size**: 10-30% of frame
**Space**: 70-90% empty or simple
**Best For**: Minimalism, isolation, scale, contemplation, modern aesthetic
**Example**: `Small subject occupies lower-right 20% of frame, remaining 80%
is sky creating negative space emphasizing isolation and scale.`

---

## Dynamic Composition Approaches

### COMP-DYN-01: Diagonal Energy
```
Subject or compositional elements positioned along diagonal lines creating
dynamic energy. Avoids horizontal/vertical stability, suggests movement,
tension, or instability. Diagonal from corner to corner most powerful.
```
**Angle**: 30-60° from horizontal typical
**Energy**: High dynamic, suggests motion or tension
**Best For**: Action, energy, instability, dynamic scenes
**Example**: `Subject positioned along diagonal from lower-left to upper-
right, creating dynamic energy and suggesting upward movement.`

---

### COMP-DYN-02: Tight Cropping
```
Subject cropped tightly, filling frame edge-to-edge. Creates intimacy,
intensity, or claustrophobia. Minimal negative space, maximum subject
presence. Emphasizes detail over context.
```
**Subject Fill**: 80-100% of frame
**Context**: Minimal or absent
**Best For**: Intimacy, intensity, detail emphasis, portraits
**Example**: `Face tightly cropped filling frame, minimal background, creates
intensity and intimacy through proximity and detail.`

---

### COMP-DYN-03: Dutch Angle (Canted)
```
Camera tilted on roll axis [15-45°] creating slanted horizon. Suggests
unease, disorientation, chaos, or stylistic punctuation. Degree of tilt
determines intensity of effect.
```
**Tilt Range**: 15-45° from level
**Psychological Effect**: Unease, disorientation, tension, style
**Best For**: Horror, unease, chaos, stylistic moments, action
**Example**: `Camera tilted 30° right creating Dutch angle, horizon slanted,
suggesting unease and disorientation in thriller scene.`

---

### COMP-DYN-04: Extreme Angles
```
Camera positioned at unusual angle: extreme low (worm's eye), extreme high
(bird's eye), or unusual perspective. Creates unique viewpoint, emphasizes
scale, or suggests POV unusual observer.
```
**Angles**: Ground-level up, overhead down, unusual perspectives
**Best For**: Unique views, scale, power dynamics, unusual POV
**Example**: `Extreme low angle from ground level looking up at subject,
emphasizing height and power, worm's eye perspective creating dominance.`

---

### COMP-DYN-05: Breaking the Frame
```
Subject partially extends beyond frame edge suggesting larger world beyond
visible frame. Creates energy, suggests incompleteness, or dynamic action.
Intentional "incorrect" framing.
```
**Technique**: Subject crop at frame edge (not fully visible)
**Best For**: Energy, dynamism, action mid-movement, larger world suggestion
**Example**: `Subject's hand extends beyond top frame edge, suggesting action
and energy beyond visible frame, dynamic incomplete composition.`

---

## Depth & Layering Composition

### COMP-DEPTH-01: Three-Plane Depth
```
Composition includes distinct foreground, middle ground, and background
elements. Creates depth through parallax, focus separation, or atmospheric
perspective. Layered visual interest.
```
**Planes**: Foreground (close), Middle (subject), Background (distant)
**Separation**: Focus, atmospheric haze, or scale
**Best For**: Depth, environmental context, layered interest
**Example**: `Foreground flowers (soft), middle ground subject (sharp),
background mountains (atmospheric haze), three-plane depth composition.`

---

### COMP-DEPTH-02: Atmospheric Perspective
```
Distant elements rendered cooler, lighter, less saturated suggesting
atmospheric haze. Creates depth through color and value shift. Natural depth
cue from atmospheric scattering.
```
**Effect**: Distant = cooler, lighter, less saturated
**Best For**: Landscapes, depth in clear subjects, natural environments
**Example**: `Distant mountains rendered cool blue and desaturated, near
elements warm and saturated, atmospheric perspective creating depth.`

---

### COMP-DEPTH-03: Overlap & Occlusion
```
Foreground elements partially obscure background creating clear depth through
layering. What's in front blocks what's behind. Simple powerful depth cue.
```
**Technique**: Foreground elements partially hide background
**Best For**: Any scene, universal depth cue, layered environments
**Example**: `Foreground tree branches partially obscure subject creating
overlap depth cue, clear front-to-back relationship established.`

---

# ATMOSPHERE & WEATHER LIBRARY

## Atmospheric Particles

### ATMO-01: Dust Motes in Light
```
Fine dust particles visible in hard light beams. Density [50-200 particles
per cubic foot visible in beam]. Creates volumetric light, shows air,
suggests age or abandonment. Particles drift slowly downward with slight
random horizontal drift.
```
**Visibility**: Requires hard directional light source
**Density**: Light (50), Medium (100), Heavy (200) particles per cu ft
**Movement**: Slow downward drift with random horizontal
**Best For**: Atmosphere, abandoned spaces, volumetric lighting
**Example**: `Dust motes visible in window light beam, medium density 100
particles per cubic foot, slow drift creating volumetric atmosphere.`

---

### ATMO-02: Light Fog/Mist
```
Atmospheric fog reducing visibility to [200-1000 feet]. Creates depth through
atmospheric haze, softens distant elements. Morning mist or light fog,
natural ground-level accumulation. Cool blue-gray color, diffuses light.
```
**Visibility Distance**: 200-1000 feet
**Color**: Cool blue-gray
**Height**: Ground to 6-10 feet typical
**Best For**: Mystery, morning scenes, depth, soft mood
**Example**: `Light morning mist reducing visibility to 500 feet, ground-
level accumulation to 8 feet, cool blue-gray creating soft mysterious mood.`

---

### ATMO-03: Heavy Fog
```
Dense fog reducing visibility to [50-200 feet]. Creates isolation, mystery,
or claustrophobia. Obscures background entirely, subject emerges from fog.
Diffuses all light creating soft directionless illumination.
```
**Visibility Distance**: 50-200 feet (dense)
**Effect**: Background obscured, isolation, mystery
**Lighting**: Diffused, soft, directionless
**Best For**: Mystery, isolation, horror, emergence scenes
**Example**: `Heavy fog reducing visibility to 100 feet, background completely
obscured, subject isolated in fog, diffused mysterious lighting.`

---

### ATMO-04: Smoke/Haze
```
Artificial smoke or atmospheric haze (not fog). Creates visible light beams,
adds texture to air. Density [light/medium/heavy]. Can be colored for effect.
Controlled atmospheric addition for film production.
```
**Source**: Fog machine/haze machine
**Density**: Light (subtle beams) to Heavy (dense atmosphere)
**Color**: Clear or tinted
**Best For**: Volumetric lighting, night scenes, concerts, mood
**Example**: `Light atmospheric haze throughout space, makes hard light
sources visible as beams, adds texture and depth to air.`

---

### ATMO-05: Rain (Light to Heavy)
```
Rain visible as [streaks/drops] in frame. Density determines visibility and
mood. Light rain: individual drops visible. Heavy rain: dense streaks
obscuring view. Creates reflections on surfaces, wet-dark aesthetic.
```
**Density**: Light (sparse drops), Medium (visible), Heavy (dense curtain)
**Visibility**: Drops as points (backlit) or streaks (side-lit)
**Effect**: Wet surfaces, reflections, darkness, mood
**Best For**: Mood, atmosphere, noir, dramatic weather
**Example**: `Medium rain visible as diagonal streaks, backlit by street
lights, creates wet reflections on pavement, noir atmospheric mood.`

---

### ATMO-06: Snow (Falling)
```
Snowflakes falling at [density]. Larger flakes (3-8mm) fall at [1-3 ft/sec],
drift with air currents. Creates winter atmosphere, softens scene, diffuses
light. Accumulation on surfaces shows duration.
```
**Flake Size**: Small (1-3mm), Medium (3-8mm), Large (8-15mm)
**Density**: Light (occasional), Medium (steady), Heavy (blizzard)
**Fall Speed**: 1-3 ft/sec with drift
**Best For**: Winter scenes, seasonal atmosphere, softening
**Example**: `Medium snowflakes falling, steady density, visible drift in
air current, creates gentle winter atmosphere and softening effect.`

---

## Weather Conditions

### WEATHER-01: Overcast Cloud Cover
```
Complete cloud cover creating diffused skylight. Shadowless even illumination,
neutral 6500K color temperature. Low contrast 2:1 to 4:1. Soft flattering
light, no harsh sun.
```
**Light Quality**: Diffused, even, shadowless
**Color Temperature**: 6000-6500K neutral
**Contrast**: 2:1 to 4:1 (very low)
**Best For**: Portraits, commercial, even illumination needs
**Example**: `Complete overcast creating natural softbox effect, shadowless
6500K illumination, 3:1 low contrast perfect for portraits.`

---

### WEATHER-02: Partly Cloudy (Dynamic)
```
Scattered clouds creating alternating sun and shade. Light changes as clouds
pass sun. Dynamic lighting conditions, requires exposure adaptation. Creates
visual variety, suggests time passing.
```
**Light Quality**: Alternating bright sun and soft cloud shade
**Variability**: Changes every 30-180 seconds
**Best For**: Dynamic scenes, time passage, natural variety
**Challenges**: Exposure changes, continuity in editing
**Example**: `Partly cloudy creating dynamic light changes, sun breaks
through clouds periodically, natural variety and time passage suggested.`

---

### WEATHER-03: Storm Approaching
```
Dark storm clouds approaching, light levels dropping. Dramatic clouds, wind
increasing, temperature drop felt. Pre-storm tension, dramatic sky. Light
from storm edge creates directional drama.
```
**Sky**: Dark dramatic clouds
**Light**: Dropping levels, directional from clear edge
**Mood**: Tension, drama, anticipation
**Best For**: Drama, tension, natural power, gothic atmospheres
**Example**: `Storm clouds approaching creating dark dramatic sky, light
levels dropping, wind increasing, pre-storm tension palpable.`

---

### WEATHER-04: Rain Wet Streets (No Active Rain)
```
Post-rain or between showers, surfaces wet and reflective. Puddles reflect
sky and lights, wet-dark aesthetic. Overcast diffused light or dramatic
clearing sky. Noir aesthetic classic condition.
```
**Surfaces**: Wet, reflective, puddles present
**Light**: Diffused or dramatic clearing
**Aesthetic**: Noir, reflective, moody
**Best For**: Noir, urban night, moody atmospheres, reflection beauty
**Example**: `Wet streets post-rain, puddles reflect neon lights, wet-dark
noir aesthetic, dramatic clearing sky with last clouds.`

---

### WEATHER-05: Golden Hour Clear
```
Clear sky 0-30 minutes after sunrise or before sunset. Warm 3200-3800K direct
sunlight, long shadows, golden glow. Ideal conditions, "magic hour" beauty.
Most flattering natural light.
```
**Sky**: Clear or minimal clouds
**Color Temperature**: 3200-3800K (warm gold)
**Shadows**: Long, dramatic, warm-edged
**Duration**: 20-40 minute window
**Best For**: Beauty, romance, optimism, landscape glory
**Example**: `Golden hour clear conditions 20 minutes before sunset, warm
3600K light creating long shadows and golden glow, magic hour beauty.`

---

# COLOR PALETTE LIBRARY

## Natural Color Palettes

### COLOR-NAT-01: Earth Tones
```
Brown #8B4513, Tan #D2B48C, Olive Green #6B8E23, Terracotta #E2725B,
Stone Gray #ADB1B8

Warm natural palette suggesting organic materials, earth, stability. Used
for natural settings, rustic environments, organic products.
```
**Mood**: Warm, natural, stable, organic, rustic
**Best For**: Nature, organic products, rustic settings, natural materials
**Example**: `Earth tone palette: brown wood #8B4513, tan leather #D2B48C,
olive foliage #6B8E23, terracotta clay #E2725B, stone #ADB1B8.`

---

### COLOR-NAT-02: Ocean/Water
```
Navy #001F3F, Deep Blue #0074D9, Cyan #7FDBFF, Aqua #39CCCC, Sea Green #2ECC40

Cool water-associated palette creating freshness, calm, or depth. Marine
environments, water products, fresh clean aesthetics.
```
**Mood**: Cool, fresh, calm, clean, deep
**Best For**: Marine environments, water, fresh products, spa/wellness
**Example**: `Ocean palette: navy depth #001F3F, water blue #0074D9, cyan
shallows #7FDBFF, aqua reef #39CCCC, sea green #2ECC40.`

---

### COLOR-NAT-03: Forest/Woodland
```
Dark Green #2C5F2D, Moss #8A9A5B, Bark Brown #654321, Fern #4F7942,
Forest Floor #3D2817

Natural forest palette suggesting growth, nature, organic life. Woodland
settings, organic products, environmental themes.
```
**Mood**: Natural, organic, growth, peaceful, grounded
**Best For**: Nature, organic products, environmental themes, woods
**Example**: `Forest palette: dark green canopy #2C5F2D, moss #8A9A5B, bark
brown #654321, fern #4F7942, forest floor #3D2817.`

---

### COLOR-NAT-04: Desert/Arid
```
Sand #F4A460, Dusty Rose #C9ADA7, Sage #9A8C98, Terracotta #E07A5F,
Adobe #C77A58

Warm muted desert palette suggesting heat, aridity, Southwest aesthetics.
Desert environments, Southwest themes, warm minimalism.
```
**Mood**: Warm, dry, minimal, Southwest, earthy
**Best For**: Desert environments, Southwest themes, warm minimalism
**Example**: `Desert palette: sand #F4A460, dusty rose #C9ADA7, sage #9A8C98,
terracotta #E07A5F, adobe #C77A58.`

---

## Cinematic Color Palettes

### COLOR-CIN-01: Teal and Orange (Blockbuster)
```
Deep Teal #16697A, Orange #FFA101, Cream #FFE6CC, Teal-Black #0A1612,
Burnt Orange #CC5500

Classic blockbuster palette creating complementary color contrast. Teal
shadows, orange highlights. Commercial cinema standard.
```
**Mood**: Cinematic, commercial, dramatic, complementary contrast
**Best For**: Action, blockbusters, commercial cinema, dramatic scenes
**Example**: `Teal and orange grade: teal shadows #16697A, orange skin tones
#FFA101, cream highlights #FFE6CC, commercial cinema standard.`

---

### COLOR-CIN-02: Bleach Bypass (Desaturated)
```
Silver Gray #C0C0C0, Muted Blue #6B8CAE, Desaturated Green #7A8B76,
Concrete #808080, Washed Red #B8575B

Desaturated high-contrast palette suggesting grit, realism, war aesthetic.
Reduced saturation -40%, increased contrast +30%.
```
**Mood**: Gritty, realistic, harsh, military, serious
**Best For**: War films, serious drama, harsh realism, dystopia
**Example**: `Bleach bypass palette: silver gray #C0C0C0, muted blue #6B8CAE,
desaturated green #7A8B76, high contrast gritty aesthetic.`

---

### COLOR-CIN-03: Film Noir Monochrome
```
Pure White #FFFFFF, Light Gray #CCCCCC, Mid Gray #808080, Dark Gray #404040,
Pure Black #000000

Monochrome palette for noir aesthetic. High contrast 16:1+, deep blacks,
hot whites. Classic noir or contemporary monochrome.
```
**Mood**: Dramatic, classic, noir, high contrast, mystery
**Best For**: Noir, mystery, classic aesthetics, dramatic contrast
**Example**: `Film noir monochrome: pure white highlights, graduated grays,
pure black shadows, 20:1 contrast creating classic noir drama.`

---

### COLOR-CIN-04: Cyberpunk Neon
```
Magenta #FF00FF, Cyan #00FFFF, Hot Pink #FF1744, Electric Blue #304FFE,
Void Black #0D0D0D

High-saturation neon colors on dark background. Cyberpunk, urban night,
tech aesthetics. Oversaturated +40% on neon sources.
```
**Mood**: Futuristic, cyberpunk, urban night, high-tech, neon
**Best For**: Cyberpunk, urban night, tech themes, neon aesthetics
**Example**: `Cyberpunk neon palette: magenta #FF00FF, cyan #00FFFF, hot
pink #FF1744 on void black #0D0D0D, oversaturated tech aesthetic.`

---

### COLOR-CIN-05: Vintage Film Stock
```
Kodak Warm #F5DEB3, Faded Red #DC7A6B, Muted Yellow #E8C84C, Sepia Shadow
#704214, Cream Highlight #FAEBD7

Warm vintage palette emulating aged film stock. Slight color shift, lifted
blacks, warm nostalgic tone. 1960s-1970s aesthetic.
```
**Mood**: Nostalgic, vintage, warm, period, faded elegance
**Best For**: Period pieces, nostalgia, vintage aesthetics, warm memories
**Example**: `Vintage film palette: Kodak warm tones, faded red, muted
yellow, sepia shadows creating nostalgic 1970s aesthetic.`

---

## Commercial/Brand Color Palettes

### COLOR-COM-01: Premium Luxury
```
Champagne Gold #F7E7CE, Deep Navy #1B2432, Burgundy #800020, Ivory #FFFFF0,
Bronze #CD7F32

Sophisticated palette suggesting luxury, premium quality, exclusivity. Muted
saturation, rich depth, elegant restraint.
```
**Mood**: Luxurious, premium, sophisticated, exclusive, elegant
**Best For**: Luxury products, high-end commercial, premium branding
**Example**: `Premium luxury palette: champagne gold accents, deep navy base,
burgundy richness, ivory highlights, sophisticated exclusivity.`

---

### COLOR-COM-02: Tech/Innovation
```
Clean White #FFFFFF, Cool Gray #E8E8E8, Accent Blue #0066FF, Highlight Cyan
#00D9FF, Dark UI #2C2C2C

Modern tech palette suggesting innovation, clarity, precision. Clean minimal
aesthetic, accent color pops on neutral base.
```
**Mood**: Modern, clean, innovative, precise, minimal
**Best For**: Tech products, innovation themes, modern commercial, UI
**Example**: `Tech innovation palette: clean white base, cool gray surfaces,
accent blue highlights, minimal modern precision aesthetic.`

---

### COLOR-COM-03: Wellness/Organic
```
Sage Green #9CAF88, Natural Beige #E8D5C4, Soft Terracotta #D4A59A,
Eucalyptus #6C9A8B, Cream #FAF9F6

Calm natural palette suggesting wellness, organic, health. Soft muted tones,
natural materials, calming effect.
```
**Mood**: Calm, natural, healthy, organic, wellness
**Best For**: Wellness products, organic brands, spa, health themes
**Example**: `Wellness palette: sage green calm, natural beige, soft
terracotta, eucalyptus, creating organic health aesthetic.`

---

### COLOR-COM-04: Energy/Sports
```
Vibrant Red #FF2D2D, Electric Yellow #FFEB3B, Dynamic Orange #FF6600,
Strong Black #1A1A1A, Pure White #FFFFFF

High-energy palette suggesting action, sports, excitement. High saturation,
strong contrast, dynamic tension.
```
**Mood**: Energetic, dynamic, exciting, athletic, bold
**Best For**: Sports products, energy brands, action themes, youth marketing
**Example**: `Energy sports palette: vibrant red action, electric yellow
highlights, dynamic orange, strong black-white contrast.`

---

### COLOR-COM-05: Food/Appetite Appeal
```
Warm Red #C1440E, Golden Yellow #FFB627, Fresh Green #7CB342, Cream #FFF8DC,
Rich Brown #5D4037

Appetite-appealing palette suggesting fresh, delicious, natural food. Warm
inviting tones, fresh accents, rich depth.
```
**Mood**: Appetizing, fresh, delicious, inviting, natural
**Best For**: Food products, restaurants, culinary themes, fresh produce
**Example**: `Food appeal palette: warm tomato red, golden bread yellow,
fresh lettuce green, cream dairy, rich chocolate brown.`

---

# TEXTURE & MATERIAL LIBRARY

## Surface Textures

### TEX-SURF-01: Brushed Metal (Aluminum)
```
Linear micro-scratches in consistent direction creating matte metallic
surface. Specular highlights elongate along grain direction. Subtle color
shift from #B8B8B8 to #D4D4D4 based on angle. Industrial precision aesthetic.
```
**Material**: Aluminum, stainless steel
**Finish**: Brushed/directional grain
**Lighting Behavior**: Elongated specular, directional highlights
**Best For**: Tech products, industrial design, modern aesthetics
**Example**: `Brushed aluminum surface with linear grain visible, specular
highlights elongate along brush direction, industrial precision finish.`

---

### TEX-SURF-02: Polished Chrome
```
Mirror-like reflective surface showing environment reflections. Specular
highlights sharp and bright. Color shifts based on reflected content. Perfect
smooth surface showing fingerprints and smudges if authentic.
```
**Material**: Chrome, polished metal
**Finish**: Mirror polish
**Lighting Behavior**: Mirror reflections, sharp specular
**Best For**: Luxury products, automotive, jewelry, high-end fixtures
**Example**: `Polished chrome surface creating mirror reflections, sharp
specular highlights, environment visible in reflection, fingerprint smudges
add authenticity.`

---

### TEX-SURF-03: Matte Black (Anodized)
```
Deep black surface absorbing light with minimal specular reflection. Slight
texture prevents perfect smoothness. No reflections, pure absorption. Modern
premium aesthetic, stealth appearance.
```
**Material**: Anodized aluminum, matte powder coat
**Finish**: Matte/non-reflective
**Lighting Behavior**: Absorbs light, minimal specular, form through shadow
**Best For**: Premium tech, stealth products, modern design
**Example**: `Matte black anodized surface absorbing light, minimal
reflection, slight texture preventing mirror finish, premium stealth
aesthetic.`

---

### TEX-SURF-04: Wood Grain (Natural)
```
Visible growth rings, grain pattern, knots. Color variation from #8B4513 to
#D2691E. Organic irregular pattern never repeating. Surface texture shows
fiber direction. Natural material character.
```
**Material**: Natural wood (oak, walnut, maple)
**Finish**: Clear coat or oil
**Pattern**: Organic growth rings, non-repeating
**Best For**: Craftsmanship, natural products, organic aesthetics
**Example**: `Natural oak wood grain visible, growth rings showing age, color
variation from dark to light, organic knot patterns, hand-crafted character.`

---

### TEX-SURF-05: Leather (Full-Grain)
```
Organic pore pattern, natural grain, color variation. Not uniform or
embossed. Shows natural hide imperfections (slight scars, color shifts).
Develops patina with use. Premium natural material character.
```
**Material**: Full-grain leather
**Pattern**: Natural pore structure, organic variation
**Aging**: Develops patina, darkens with use
**Best For**: Luxury goods, craftsmanship, premium products
**Example**: `Full-grain leather showing natural pore structure, organic
color variation, slight scar marks proving authenticity, developing warm
patina from use.`

---

### TEX-SURF-06: Concrete (Raw/Exposed)
```
Rough texture, visible aggregate, surface imperfections. Color #808080 to
#A9A9A9 with variation. Porous surface, slight edge chips. Industrial
brutalist aesthetic. Unfinished raw character.
```
**Material**: Poured concrete
**Finish**: Raw/unsealed
**Texture**: Rough, porous, imperfect
**Best For**: Industrial, brutalist, raw aesthetics, urban environments
**Example**: `Raw concrete surface showing aggregate texture, edge chips,
color variation, porous unfinished character, industrial brutalist
aesthetic.`

---

### TEX-SURF-07: Fabric Weave
```
Visible thread weave pattern, individual fibers discernible. Weave creates
directional texture affecting light. Fabric type determines pattern: canvas
(tight regular), linen (irregular organic), silk (fine smooth).
```
**Material**: Canvas, linen, silk, cotton
**Pattern**: Weave structure visible
**Scale**: Macro detail shows individual threads
**Best For**: Textile products, fashion, craftsmanship detail
**Example**: `Canvas fabric weave visible in macro, individual threads
discernible, tight regular pattern creating subtle directional texture.`

---

### TEX-SURF-08: Glass (Transparent)
```
Transparent with subtle specular highlights and refractions. Edge thickness
visible. Fingerprints and smudges if authentic. Light passes through with
slight color tint (green edge typical). Reflections on both surfaces.
```
**Material**: Glass, crystal
**Finish**: Polished smooth
**Behavior**: Transparent, refractive, reflective
**Best For**: Glassware, windows, transparency demonstrations
**Example**: `Clear glass transparent with slight green tint at edges,
specular highlights on surfaces, subtle fingerprint smudges, light refraction
visible.`

---

## Wear & Aging Textures

### TEX-WEAR-01: Scratched Surface
```
Multiple fine scratches visible on painted or coated surface. Scratches vary
in depth, length, direction. Shows history of use. Ranging from surface
marks to exposed base material. Realistic wear pattern.
```
**Effect**: Surface damage from use
**Pattern**: Random direction, varying depth
**Best For**: Authenticity, aged items, used equipment, realism
**Example**: `Paint surface showing multiple scratches varying depth,
random directions suggesting authentic use history, some expose metal beneath.`

---

### TEX-WEAR-02: Patina/Oxidation
```
Metal surface showing oxidation or patina. Copper: green verdigris. Brass:
brown-green tarnish. Steel: rust orange-brown. Uneven coverage suggesting
exposure variation. Natural aging beauty.
```
**Materials**: Copper, brass, bronze, steel
**Color**: Material-specific oxidation color
**Pattern**: Uneven, concentrated at edges and crevices
**Best For**: Age, authenticity, vintage items, outdoor exposure
**Example**: `Brass surface showing natural patina, green-brown tarnish
concentrated at edges and crevices, uneven coverage from varied exposure.`

---

### TEX-WEAR-03: Worn Edges
```
High-contact edges showing finish wear to base material. Paint worn through
at handle areas, corners, edges. Reveals use patterns and touch frequency.
Polishing from hand contact creating shine on worn areas.
```
**Location**: Edges, corners, handles, high-contact points
**Effect**: Finish removal, base material exposed, polishing
**Best For**: Authenticity, tools, handled objects, antiques
**Example**: `Tool handle edges worn through paint to bare wood, polished
smooth from hand contact, showing use pattern and touch frequency.`

---

### TEX-WEAR-04: Faded/Sun-Damaged
```
Color fading from UV exposure. Originally bright colors muted to pastels or
gray. Uneven fading showing shadow patterns. Fabric shows fiber damage,
brittle texture. Paint chalking visible.
```
**Cause**: UV/sun exposure over time
**Effect**: Color desaturation, uneven patterns, material degradation
**Best For**: Outdoor items, vintage, age demonstration, weather exposure
**Example**: `Fabric faded from sun exposure, originally red now pale pink,
uneven fading showing window shadow pattern, fibers brittle from UV damage.`

---

### TEX-WEAR-05: Water Damage/Staining
```
Water stains creating irregular organic patterns. Color darkening, edge
definition, mineral deposits. Warping in wood/paper. Mold/mildew growth in
severe cases. Authentic deterioration patterns.
```
**Effect**: Staining, warping, degradation
**Pattern**: Organic irregular, edge-defined rings
**Best For**: Abandoned spaces, age, neglect, authentic deterioration
**Example**: `Ceiling tile showing water damage stain, irregular organic
pattern with defined dark edges, slight warping, mildew spots in heavy areas.`

---

# TIME & SPEED CONTROL LIBRARY

## Frame Rate & Playback Speed

### TIME-01: 24fps Cinema Standard
```
Captured at 24fps, played at 24fps. Real-time cinema standard creating
natural motion with characteristic motion blur at 180° shutter. Cinematic
look, slight judder on pans (inherent to format), film aesthetic.
```
**Capture**: 24fps
**Playback**: 24fps
**Speed**: 1.0x (real-time)
**Aesthetic**: Cinematic, film-like, traditional
**Best For**: Narrative film, cinematic content, theatrical release
**Example**: `24fps cinema standard capture and playback, real-time with
cinematic motion blur, characteristic film aesthetic and slight pan judder.`

---

### TIME-02: 30fps Broadcast Smooth
```
Captured at 30fps (29.97fps NTSC), played at 30fps. Slightly smoother than
cinema, broadcast television standard. Less motion blur than 24fps, different
aesthetic. TV/broadcast look.
```
**Capture**: 30fps (29.97fps NTSC)
**Playback**: 30fps
**Speed**: 1.0x (real-time)
**Aesthetic**: Broadcast smooth, TV standard
**Best For**: Broadcast television, NTSC content, news, sports
**Example**: `30fps broadcast standard, slightly smoother than cinema,
traditional television aesthetic, NTSC compatibility.`

---

### TIME-03: 60fps High Frame Rate
```
Captured at 60fps, played at 60fps. Very smooth motion, minimal blur,
hyper-real "video" aesthetic. Not cinematic, modern digital look. Excellent
for sports, action detail, or modern commercial.
```
**Capture**: 60fps
**Playback**: 60fps
**Speed**: 1.0x (real-time)
**Aesthetic**: Hyper-smooth, modern, "video look"
**Best For**: Sports, gaming, action detail, modern commercial, vertical
**Example**: `60fps high frame rate, ultra-smooth motion, hyper-real modern
aesthetic, excellent action detail, minimal motion blur.`

---

### TIME-04: 120fps Subtle Slow-Motion
```
Captured at 120fps, conformed to 24fps playback. 5x slow-motion (20% speed).
Reveals details in fast action, gentle slow-motion aesthetic. Not extreme,
maintains some action speed while adding weight.
```
**Capture**: 120fps
**Playback**: 24fps
**Speed**: 0.2x (20% / 5x slow)
**Aesthetic**: Gentle slow-motion, action detail
**Best For**: Action moments, impacts, reveals, gentle emphasis
**Example**: `120fps conformed to 24fps creating 5x gentle slow-motion,
reveals action details while maintaining drama, not extreme slowness.`

---

### TIME-05: 240fps Dramatic Slow-Motion
```
Captured at 240fps, conformed to 24fps playback. 10x slow-motion (10% speed).
Freezes fast action, reveals micro-details, dramatic emphasis. Obvious slow-
motion creating beauty or drama in motion.
```
**Capture**: 240fps
**Playback**: 24fps
**Speed**: 0.1x (10% / 10x slow)
**Aesthetic**: Dramatic slow-motion, frozen details
**Best For**: Impacts, water/fluid, emotional peaks, beauty in motion
**Example**: `240fps conformed to 24fps creating 10x dramatic slow-motion,
water droplets frozen mid-air, emotional peak emphasized, beauty revealed.`

---

### TIME-06: Time-Lapse (Variable Acceleration)
```
Captured at 1 frame per [X seconds], played at 24fps. Extreme acceleration
showing time passage. Clouds race, sun arcs, crowds blur. Compression ratio
determines speed (1 frame/10sec = 240x acceleration at 24fps playback).
```
**Capture**: 1 frame per X seconds
**Playback**: 24fps
**Speed**: 240x to 10,000x+ (varies by interval)
**Aesthetic**: Hyper-accelerated, time passage, natural cycles
**Best For**: Time passage, construction, nature cycles, city energy
**Example**: `Time-lapse 1 frame every 10 seconds over 2 hours, played at
24fps creates 4-minute sequence, 30x acceleration showing sunset compressed.`

---

---

**END OF MODULAR COMPONENTS LIBRARY**

*These components can be mixed and matched with any base template from the
Master Prompt Library. Simply copy the relevant component description and
insert into your template at the appropriate position.*

*Next sections: Style Presets and Complete Usage Workflows*
