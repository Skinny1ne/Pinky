# PINKY PINKY - Cinematic Effects Quick Reference

## How to Use the Cinematic Functions

### Basic Fade Transitions
```javascript
// Fade to black and wait
await fadeToBlack(1500);
// ... do something ...
// Fade back in
await fadeFromBlack(1500);
```

### Jumpscare Effects
```javascript
// Complete jumpscare with all effects
await jumpscareSequence();
// Then trigger game over
gameOver("caught");
```

### Screen Effects During Gameplay

#### Screen Shake (for impacts/fear)
```javascript
// Moderate shake
screenShake(2, 300); // Intensity 2, 300ms

// Intense shake  
await screenShake(4, 500); // Intensity 4, 500ms
```

#### Glitch Effect (for Pinky presence)
```javascript
// Moderate glitch
glitchEffect(500, 1); // 500ms, intensity 1

// Severe glitch
glitchEffect(1000, 3); // 1000ms, intensity 3
```

#### Reality Distortion
```javascript
// Makes screen warp and shift
distortionEffect(1000, 1); // 1000ms, intensity 1
```

#### Red Flash (danger indicator)
```javascript
// Quick red flash
redFlashEffect(200, 1); // 200ms, intensity 1

// Intense red flash
redFlashEffect(300, 2); // 300ms, intensity 2
```

### Complex Multi-Effect Sequences

#### Pursuit Sequence (full intensity)
```javascript
// Combines multiple effects over 5 seconds
await pursuitEffects(5000);
```

#### Cinematic Letterbox
```javascript
// Show black bars
showCinematicBars();
// ... perform action ...
// Hide bars
hideCinematicBars();
```

### Individual Frame Effects

#### Reality Warp (one-shot)
```javascript
// Used during continuous threat
realityWarpEffect(0.5); // Intensity 0.5
```

#### Breath Fog (hiding effect)
```javascript
// Creates visible breath effect
breathFogEffect();
```

#### Portal Effect
```javascript
// Glitch when portal opens
mirrorPortalEffect();
```

---

## Integration Examples

### Example 1: Chase Sequence
```javascript
// In your game loop, when Pinky is close
if (distanceToPinky < 10) {
    // Subtle effect every frame
    realityWarpEffect(0.3);
}

// When very close
if (distanceToPinky < 5) {
    // More intense
    distortionEffect(500, 0.8);
}
```

### Example 2: Mirror Encounter
```javascript
async function playerLooksMirror() {
    showCinematicBars();
    mirrorPortalEffect();
    
    // Pinky appears
    await new Promise(r => setTimeout(r, 500));
    
    await jumpscareSequence();
    gameOver("mirror");
}
```

### Example 3: Escape Route Found
```javascript
async function foundExit() {
    // Dramatic transition
    await fadeToBlack(800);
    
    // Victory sequence
    gameWon("THE TALE (DOOR)");
    
    await fadeFromBlack(1000);
}
```

### Example 4: Fear Buildup
```javascript
// Gradual fear escalation
let fearLevel = player.fearLevel; // 0 to 1

if (fearLevel > 0.5) {
    // Moderate effect
    distortionEffect(300, fearLevel * 1.5);
}

if (fearLevel > 0.8) {
    // Intense pursuit effects
    screenShake(fearLevel * 3, 200);
}

if (fearLevel > 0.95) {
    // Imminent capture
    await pursuitEffects(2000);
}
```

---

## Effect Parameters Reference

### Effect Intensities
- **0.1-0.5**: Subtle, almost unnoticeable
- **0.5-1.0**: Noticeable but manageable
- **1.0-2.0**: Obvious, creates tension
- **2.0-3.0**: Very intense, disorienting
- **3.0+**: Extreme, may cause discomfort (use sparingly)

### Duration Guidelines
- **100-200ms**: Quick flash/blink effects
- **300-500ms**: Single event effects
- **500-1000ms**: Sustained effects
- **1000-2000ms**: Transition effects
- **2000+**: Scene transitions or sequences

### Best Practices
1. Use `await` for sequential effects
2. Don't overlap same effect types (e.g., two glitches)
3. Keep intense effects under 1 second
4. Always provide escape path for player (stop effects on death)
5. Test on target hardware for performance

---

## CSS Class Applications

All cinematics are applied via:
- Direct style manipulation: `element.style.filter = ...`
- CSS animations: `element.style.animation = ...`
- CSS classes: `element.classList.add('show')`

No external CSS libraries required - pure vanilla JavaScript!

---

## Browser Compatibility

- ✅ Chrome/Edge (v70+)
- ✅ Firefox (v68+)
- ✅ Safari (v12+)
- ✅ Opera (v57+)
- ⚠️ Mobile browsers (varies by device)

Most effects use:
- `requestAnimationFrame` (universal)
- `CSS Filter` (wide support)
- `Transform` (wide support)
- `setTimeout/setInterval` (universal)

---

## Performance Tips

1. **Throttle effects**: Don't apply multiple effects every frame
2. **Use requestAnimationFrame**: Already implemented in all functions
3. **Clean up**: Effects auto-cleanup after duration
4. **Test FPS**: Monitor performance on target devices
5. **Reduce intensity**: Lower values = better performance

---

## Troubleshooting

**Effects not showing?**
- Check z-index is high enough
- Verify DOM element exists (`#hud`, etc.)
- Check browser console for errors
- Ensure Three.js renderer is rendering

**Audio out of sync?**
- Jumpscare audio is triggered in `jumpscareSequence()`
- Adjust timing in sound functions if needed

**Shaking too intense?**
- Reduce intensity parameter (use 1-2 instead of 3-4)
- Reduce duration (300ms instead of 500ms)

**Frame rate drops?**
- Reduce glitch intensity
- Limit effect frequency to key moments
- Use lower duration values

---

**For more details, see: CINEMATICS_FEATURES.md**
