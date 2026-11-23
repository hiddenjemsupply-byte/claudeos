# Jemfall: The Guide

Status: concept. Recommended pick is Glint. Rough sketch: game/art/glint-concept.png

## The Job
* **In the game:** teaches new players, answers "what do I do next," explains what any item is for. This is the fix for OSRS and Melvor being hard to get into.
* **On social:** the face of Jemfall. Every clip is the Guide talking to the audience through a pixel text box.

## What Makes a Mascot Work
* Recognizable as a plain black silhouette, with no detail
* Simple shapes, few small parts
* A limited palette with one standout color and a dark outline
* Works tiny (map sprite) and big (profile picture, thumbnails)

## Three Concepts

### 1. Glint (recommended)
A shard of the first Jem that fell, which woke up. It's been through every rift, knows everything, and is mildly worried about you.
* **Why it wins:** the silhouette is a gem shape with eyes, so it passes the silhouette test instantly. It uses the Jem color, so the mascot, the currency, and the brand become one picture. It's easy to animate: floating, bobbing, sparkling. It comes straight from the Jemfall story.
* **Bonus:** it's literally made of Jem, and it tells players Jems never buy power. The mascot becomes the proof that the game isn't pay to win.

### 2. The Cartographer
An old hooded explorer with a huge backpack of maps and a lantern, who has stepped through every rift.
* Classic, warm, and easy to understand. But it's the most generic option. Terraria's Guide is already an ordinary guy.

### 3. Moss
A small stone golem with a Jem crystal stuck in its head, grown over with moss.
* Fits the world and has charm, but a rock body is hard to read at small sizes and harder to animate.

## Glint: Full Spec

### Look
* Faceted gem body in the Jem colors, two big eyes, tiny stubby arms, always floating
* Colors: #C837D6 body, #8A1E8C shadow, #EE6BF0 light, #FFC6FB shine, #2E222F outline and pupils, #FFFFFF eye whites. Nothing else.
* Dark outline on everything

### Sizes
* **Portrait 64x64:** for the text box and social clips. Same portrait size Stardew Valley uses. This is the master design.
* **Map sprite 16x16:** floats next to the player on the map
* **Profile picture:** portrait scaled up on the dark background, replacing the plain Jem later

### Expressions (portrait)
Neutral, happy, worried, deadpan, shocked, proud. Six covers almost every line.

### Animations
* Idle float: gentle bob up and down (4 frames)
* Talk: mouth open and close (2 to 3 frames)
* Blink
* Excited: quick spin with sparkles
* Worried: small wobble

### Personality
* Deadpan and honest to a fault
* A little anxious about the player, in a caring way
* Dry, short jokes. Never more than three short lines at a time.
* Never sells anything. It will happily say Jems can't buy power.

### Voice
* Small, quick, slightly bright. Not squeaky, not a cartoon chipmunk.
* Record lines in a calm, flat, deadpan tone. The voice changer handles the sound. The timing is what makes it funny.
* In ElevenLabs, test 3 light, youthful voices from the voice library on the same line and pick by ear. Then never change it.

### Sample Lines
* "Nope. Your skills keep going forever. I've seen someone chop trees for a week. I worry about them."
* "The shiny pink things that fell from the sky? That's my family. You can buy outfits with them. You can't buy power. I checked."
* "The further you get from home, the darker it gets. That's not a metaphor. Bring a torch."
* "Every 3 months, everybody starts fresh. You keep your cosmetics. You lose your excuses."
* "Stuck? That's what I'm for. Tap me."

## PixelLab Prompts
Generate the portrait first. Once one is approved, use it as the reference for everything else so Glint always looks like Glint.

**Portrait (64x64, master)**
> Cute small living gem creature mascot named Glint. Body is a faceted cut gem in bright pink purple, shaped like a classic diamond icon, wider at the top and coming to a point at the bottom. Two large expressive eyes with white whites and dark pupils, a small simple mouth, tiny stubby arms on the sides. Floating. Front view. Thick dark purple black outline, simple cel shading with a bright shine on the upper left facet. Limited palette: #C837D6, #8A1E8C, #EE6BF0, #FFC6FB, #2E222F, #FFFFFF. 16 bit pixel art, transparent background.

**Expressions (64x64, same reference)**
> Same character, [happy / worried / deadpan with half closed eyes / shocked with wide eyes / proud with chin up] expression. Keep body shape, colors, and outline identical.

**Map sprite (16x16)**
> Tiny floating gem creature, pink purple faceted gem with two eyes, dark outline, same palette as reference, 16x16 pixel art, 4 directions, transparent background.

**Animations**
> Idle: gently bobbing up and down, floating, 4 frames.
> Talk: mouth opening and closing while floating.
> Blink: eyes close and open.

## Kling Prompts (teaser shots)
Use a PixelLab image as the start frame. Keep motion slow so the pixels stay crisp.

**Shot 1: the fall**
> Pixel art scene. A glowing pink purple gem falls from a dark starry night sky and crashes into a green grass field. The ground cracks and a glowing pink rift tears open. Slow camera, crisp pixel art, no motion blur.

**Shot 2: Glint wakes up**
> Pixel art. A small pink purple gem creature in the grass slowly opens its eyes, blinks, and looks at the camera. Subtle, slow motion. Crisp pixel art, no motion blur.

## After It's Made
* Clean every final frame to the pixel grid and the palette above
* Save the approved portrait as the master reference
* Swap the social profile pictures to Glint

## Sources
* Silhouette test: https://www.creativebloq.com/art/character-design/how-to-design-instantly-recognisable-characters-using-strong-silhouettes
* Limited palette and dark outline for mascots: https://www.freelancer.com/articles/graphic-design/good-character-design
* Stardew portrait size (64x64): https://forums.stardewvalley.net/threads/sprite-size-first-time-modding-sv.7128/latest
* PixelLab sizes and prompt contents (third party wiki): https://sorceress.games/wiki/wizard-genie/pixellab-and-sprites
* PixelLab character creator (4 or 8 directions): https://www.pixellab.ai/llms-full.txt
* Kling: keep motion slow on pixel art: https://kling.ai/topics/animate-pixel-art-ai
