# PINKY PINKY - Cinematic Features Added

## Overview
Your `pinky.html` file has been enhanced with comprehensive cinematic effects and animations to create a more immersive horror experience.

---

## CSS Animations Added

### Visual Effects Keyframes

1. **cinematicBarIn / cinematicBarOut**
   - Letterbox-style black bars sliding in/out for cinematic scenes
   - Used for dramatic transitions

2. **cinematicZoom**
   - Slow zoom effect (1 to 1.05 scale)
   - Creates tension and intensity

3. **cinematicDistortion**
   - Screen brightness and contrast shifts
   - Creates disorientation during intense moments

4. **glitchEffect**
   - Multi-layer glitch animation with clip-path and translate
   - Used for reality distortions when Pinky is near

5. **redFlash**
   - Intense red screen flash for jumpscares
   - Opacity pulses from 0 to 0.6

6. **textReveal**
   - Text slowly reveals with letter-spacing animation
   - Used for dialogue and important messages

7. **cameraShake**
   - Multi-axis screen shake with rotation
   - Applied during jumpscares and intense moments

8. **slowMotionPulse**
   - Pulsing opacity effect for slow-motion sequences

9. **ritualGlow**
   - Glowing text shadow that scales and intensifies
   - Used during the ritual sequence

10. **mirrorPortalShimmer**
    - Portal shimmer effect with blur transitions
    - Indicates magical mirror locations

11. **breathFog**
    - Breath fog visual that fades and rises
    - Used when hiding and holding breath

12. **realityWarp**
    - Reality distortion with blur and brightness shifts
    - Indicates Pinky's presence

13. **cinematicColorShift**
    - Hue rotation effect for atmosphere changes
    - Creates reality instability

14. **bloodDrip**
    - Blood effect animation for horror moments

15. **pinkyEmerge**
    - Pinky's emergence animation with scale and opacity
    - Dramatic entrance

16. **dialogueSlideIn**
    - Dialogue box slides in from bottom with fade
    - Smooth, cinematic text presentation

17. **pursuitIntensify**
    - Multi-effect pursuit sequence combining brightness, contrast, and glow
    - Indicates extreme danger

---

## JavaScript Functions Added

### Core Cinematic Functions

#### `showCinematicBars() / hideCinematicBars()`
- Display/hide letterbox bars for cinematic sequences
- Creates immersive framing effect

#### `fadeToBlack(duration) / fadeFromBlack(duration)`
- Promise-based fade effects
- Async/await compatible for sequencing events
- Default duration: 1500ms

#### `glitchEffect(duration, intensity)`
- Creates screen glitch with random brightness/contrast/hue shifts
- Parameters:
  - `duration`: Effect length in ms
  - `intensity`: How severe the glitch is (0-3+)

#### `screenShake(intensity, duration)`
- Shakes the HUD with random translation
- Parameters:
  - `intensity`: Shake magnitude (1-4)
  - `duration`: Effect length in ms
- Returns Promise for sequencing

#### `redFlashEffect(duration, intensity)`
- Red screen flash for danger/jumpscares
- Parameters:
  - `duration`: Flash length in ms
  - `intensity`: How red (0-1+)

#### `slowMotionEffect(duration, speedMultiplier)`
- Slows game time perception
- Currently placeholder-ready for physics manipulation

#### `distortionEffect(duration, intensity)`
- Reality warping blur/brightness shifts
- Creates disturbing visual effect

#### `colorShiftEffect(targetColor, duration)`
- Shifts screen color (e.g., to red)
- Parameters:
  - `targetColor`: 'red', 'blue', etc.
  - `duration`: Transition length in ms

#### `pursuitEffects(duration)`
- Complex multi-phase pursuit sequence
- Combines distortion, shakes, glitch, and flashes
- Async/await compatible

#### `jumpscareSequence(pinkyDistance)`
- Complete jumpscare with:
  - Audio trigger
  - Extreme camera shake
  - Multiple red flashes
  - Glitch effect
- Async/await ready

#### `mirrorPortalEffect()`
- Glitch effect with cinematic bars
- Used when portals activate

#### `realityWarpEffect(intensity)`
- One-shot reality warp with blur/brightness
- Used continuously when Pinky nearby

#### `breathFogEffect()`
- Creates visual breath fog that fades out
- Adds immersion to hiding mechanic

#### `textRevealEffect(element, duration)`
- Text slowly reveals with animation
- Used for dramatic dialogue

#### `createBloodTexture()`
- Creates procedural blood splatter texture
- Uses canvas to generate splatter pattern
- Used for visual effects

---

## Integration Points

### 1. **Game Over Sequence**
```javascript
gameOver(reason)
```
- Calls `jumpscareSequence()` for cinematic death
- Red flash overlay
- Fade to black before end screen

### 2. **Game Won Sequence**
```javascript
gameWon(title)
```
- Fade to black (1000ms)
- Transition to end screen
- Fade from black for cinematic victory

### 3. **The Shift (Intro to Game)**
```javascript
triggerTheShift()
```
Enhanced with:
- Show cinematic bars
- Fade to black
- World groan sound
- Level rebuild
- Fade from black
- Hide cinematic bars

### 4. **Fear/Pursuit Moments**
Can trigger during active gameplay:
- `pursuitEffects()` - Complete pursuit sequence
- `distortionEffect()` - Reality warping
- `realityWarpEffect()` - Continuous Pinky presence effect

### 5. **Dialogue Moments**
- Dialogue boxes auto-animate in with `dialogueSlideIn`
- Text reveal effects optional via `textRevealEffect()`

---

## Cinematic Sequence Examples

### Example 1: Jumpscare
```javascript
// When Pinky catches player
async function handleCapture() {
    await jumpscareSequence();
    gameOver("caught");
}
```

### Example 2: Escape Sequence
```javascript
// When player finds exit
async function handleEscape() {
    await fadeToBlack(1000);
    // Load end screen
    gameWon("THE TALE (DOOR)");
    await fadeFromBlack(1000);
}
```

### Example 3: Pursuit Effect
```javascript
// During active chase
async function activatePursuit() {
    pursuitEffects(5000); // 5 second intense sequence
}
```

---

## Visual Hierarchy

The cinematics are layered with proper z-index management:
- HUD Effects: z-index 10-15
- Cinematic Bars: z-index 301
- Fade Overlay: z-index 999
- Jumpscare Overlay: z-index 9998
- End Screen: z-index 200

---

## Performance Considerations

- All effects use `requestAnimationFrame` for smooth performance
- Effects are cancellable and promise-based for proper sequencing
- Glitch effects use reasonable duration defaults
- Screen shakes use delta timing for frame-independent motion

---

## Future Enhancement Ideas

1. **Pinky-specific cinematics** when she gets close
2. **Mirror shattering** effect when using mirrors
3. **Footstep particle effects** for visibility
4. **Breath misting** in cold areas
5. **Blood smears** on surfaces
6. **Creature design cinematics** with decals
7. **Physics-based knockback** on jumpscare
8. **Audio frequency manipulation** during fear
9. **Adaptive difficulty** based on cinematic triggers
10. **Replay cinematics** from highlights

---

## Testing Recommendations

1. Test fade transitions with varying durations
2. Verify glitch effect doesn't cause motion sickness (moderate intensity)
3. Screen shake on different refresh rates (60Hz, 144Hz, etc.)
4. Audio sync with visual jumpscare effects
5. Dialogue box animations on slow devices
6. Cinematic bar rendering on mobile/tablet

---

**Last Updated:** November 12, 2025
**Version:** Enhanced with Full Cinematic System
