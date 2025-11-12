This file contains all comments extracted from `pinky.html`.

Format: [Type] location snippet

---

<!-- HTML comments -->

- At top: none beyond those inside the imported content.

/* CSS and JS block comments and inline comments below are taken verbatim from the original file. */

---

CSS / Inline comments and JS comments from pinky.html:

1. CSS: "/* --- Base Theme & Custom Cursor --- */"
2. CSS: "/* Hide default cursor */"
3. CSS: "/* Center on cursor pos */"
4. CSS: "/* Hidden by default */"
5. CSS: "/* --- Loading Screen --- */"
6. CSS: "/* --- Menu Screens --- */"
7. CSS: "/* Lines 140-143 omitted */"
8. CSS: "/* Lines 309-314 omitted */"
9. CSS: "/* Lines 602-604 omitted */"
10. CSS: "/* Lines 606-608 omitted */"
11. CSS: "/* Lines 613-615 omitted */"
12. CSS: "/* Lines 617-619 omitted */"
13. CSS: "/* Lines 625-626 omitted */"
14. CSS: "/* Lines 628-629 omitted */"
15. CSS: "/* Lines 635-636 omitted */"
16. CSS: "/* Lines 638-639 omitted */"
17. CSS: "/* Lines 641-642 omitted */"
18. CSS: "/* Lines 644-645 omitted */"
19. CSS: "/* Lines 647-648 omitted */"
20. CSS: "/* Lines 654-656 omitted */"
21. CSS: "/* Lines 658-660 omitted */"
22. CSS: "/* Lines 662-664 omitted */"
23. CSS: "/* Lines 666-668 omitted */"
24. CSS: "/* Lines 670-672 omitted */"
25. CSS: "/* Lines 674-676 omitted */"
26. CSS: "/* Lines 682-683 omitted */"
27. CSS: "/* Lines 685-686 omitted */"
28. CSS: "/* Lines 688-689 omitted */"
29. CSS: "/* Lines 695-697 omitted */"
30. CSS: "/* Lines 699-701 omitted */"
31. CSS: "/* Lines 707-708 omitted */"
32. CSS: "/* Lines 710-711 omitted */"
33. CSS: "/* Lines 713-714 omitted */"
34. CSS: "/* Lines 716-717 omitted */"
35. CSS: "/* Lines 719-720 omitted */"
36. CSS: "/* Lines 722-723 omitted */"
37. CSS: "/* Lines 725-726 omitted */"
38. CSS: "/* Lines 728-729 omitted */"
39. CSS: "/* Lines 731-732 omitted */"
40. CSS: "/* Lines 734-735 omitted */"
41. CSS: "/* Lines 741-742 omitted */"
42. CSS: "/* Lines 744-745 omitted */"
43. CSS: "/* Lines 751-753 omitted */"
44. CSS: "/* Lines 755-757 omitted */"
45. CSS: "/* Lines 759-761 omitted */"
46. CSS: "/* Lines 767-769 omitted */"
47. CSS: "/* Lines 771-773 omitted */"
48. CSS: "/* Lines 775-777 omitted */"
49. CSS: "/* Lines 783-785 omitted */"
50. CSS: "/* Lines 787-788 omitted */"
51. CSS: "/* Lines 790-792 omitted */"
52. CSS: "/* Lines 798-799 omitted */"
53. CSS: "/* Lines 801-802 omitted */"
54. CSS: "/* Lines 804-805 omitted */"
55. CSS: "/* Lines 807-808 omitted */"
56. CSS: "/* Lines 810-811 omitted */"
57. CSS: "/* Lines 817-818 omitted */"
58. CSS: "/* Lines 820-821 omitted */"
59. CSS: "/* Lines 823-824 omitted */"
60. CSS: "/* Lines 830-831 omitted */"
61. CSS: "/* Lines 833-834 omitted */"
62. CSS: "/* Lines 840-842 omitted */"
63. CSS: "/* Lines 844-845 omitted */"
64. CSS: "/* Lines 847-849 omitted */"
65. CSS: "/* Lines 855-857 omitted */"
66. CSS: "/* Lines 859-861 omitted */"
67. CSS: "/* Lines 871-873 omitted */"
68. CSS: "/* Lines 875-877 omitted */"
69. CSS: "/* Lines 879-881 omitted */"
70. CSS: "/* Lines 883-885 omitted */"

---

JS comments and in-file annotations:

1. "// NEW: Import DecalGeometry"
2. "// --- Custom cursor logic ---"
3. "// --- Global Game State ---"
4. "// Peek configuration (tweakable)"
5. "// Helper: pick a corner spawn near the player from collidables (returns THREE.Vector3 or null)"
6. "// --- DOM Elements ---"
7. "// --- NEW: Texture Loaders and Helper Functions ---"
8. "/* Create a blood splatter texture using canvas */"
9. "// --- Sound System (Tone.js) ---"
10. "// Robustness: if the Tone.js script reported a load failure, immediately fallback"
11. "// Immediate fallback if script onerror fired"
12. "// Otherwise retry a few times (shorter timeout) before falling back"
13. "// START Tone audio context"
14. "// FIX: Ensure AudioContext is started on user gesture (handled by play button)"
15. "// We just define the synths here"
16. "// Show a small HUD indicator when audio is unavailable"
17. "// Find a nearby non-colliding spawn point around origin by sampling offsets."
18. "// Returns a THREE.Vector3 or null if none found."
19. "// --- Dialogue System ---"
20. "// NEW: Message box for item/info messages"
21. "// --- Player Class (NEW MOVEMENT) ---"
22. "// FIX: Check for Enter key during intro and playing states"
23. "// Allow Enter to close message boxes"
24. "// Allow Enter to advance dialogue during gameplay"
25. "// Developer / debug: summon Pinky in front of player"
26. "// Don't need to handle Enter during intro on key up"
27. "// Don't interfere with gameplay key ups"
28. "// RMB"
29. "// LMB"
30. "// NEW: Traditional Movement Logic"
31. "// FIX: Corrected movement directions"
32. "// Ignore camera pitch"
33. "// Apply direction relative to camera"
34. "// Check X-axis collision"
35. "// Debug: movement blocked by collision on X"
36. "// Check Z-axis collision"
37. "// Debug: movement blocked by collision on Z"
38. "// Sound"
39. "// NEW: Flashlight"
40. "// NEW: Speed up AI timer"
41. "// --- Pinky AI Class (NEW SLOW BURN) ---"
42. "// Start hiss loop"
43. "// Start aggressive sooner (30s ambient instead of 120s)"
44. "// Make prowling resume on a consistent 20s cadence to match request"
45. "// Keep prowl duration around 20s so Pinky walks around every ~20s"
46. "// Legacy state"
47. "// Don't catch player if they're hiding"
48. "// Trigger jumpscare sequence"
49. "// Make Pinky peek from a mirror trap: appear at the mirror's spawnPoint for a short time."
50. "// Accept either a mirror object with userData.spawnPoint or a pseudo object with spawnPoint"
51. "// fallback"
52. "// If spawn is null, try to find one near player"
53. "// Clear any existing peek timeout"
54. "// Auto-hide after configured ms if not interacted with"
55. "// small shake before disappearance to add tension"
56. "// NEW: High window with \"god rays\""
57. "// Dripping water sound effect - play every 2-4 seconds"
58. "// --- Game Loop ---"
59. "// Track per-mirror look timers: if player looks directly at a lethal mirror (within flashlight range) for 3s, trigger a peek"
60. "// subtle shimmer to telegraph peek when approaching 2s"
61. "// shimmer when approaching the trigger threshold"
62. "// probabilistic roll"
63. "// failed the probability roll; small cooldown to avoid immediate retrigger"
64. "// --- Mirror Logic ---"
65. "// --- Lethal Mirror Trap Logic ---"
66. "// If player directly looks at Pinky while he is peeking, make him disappear within 2s"
67. "// Reset timers for mirrors not being looked at"
68. "// --- Item/Door Logic ---"
69. "// --- Window & State Management ---"
70. "// Defensive fallback: ensure keyboard movement remains enabled even when pointer lock is not active"
71. "// Do not request pointer lock automatically; require user click."
72. "// Pointer lock requests must come from user gestures in many browsers."
73. "// Defensive fallback: ensure player controls unlocked so keyboard movement works even without pointer lock"
74. "// --- Start Init ---"

---

End of extracted comments.


---
Extracted on: 2025-11-12T18:56:36.224221Z
Total comments found: 285


[1] Type: HTML
<!-- Cinematic Bars for immersive transitions -->


[2] Type: HTML
<!-- Message box for item pickups and info -->


[3] Type: BLOCK
/* --- Base Theme & Custom Cursor --- */


[4] Type: BLOCK
/* Hide default cursor */


[5] Type: BLOCK
/* Center on cursor pos */


[6] Type: BLOCK
/* Hidden by default */


[7] Type: BLOCK
/* --- Loading Screen --- */


[8] Type: BLOCK
/* --- Menu Screens --- */


[9] Type: BLOCK
/* --- In-Game HUD --- */


[10] Type: BLOCK
/* --- Cinematic Elements --- */


[11] Type: BLOCK
/* Slow zoom cinematic */


[12] Type: BLOCK
/* Distortion effect */


[13] Type: BLOCK
/* Glitch effect */


[14] Type: BLOCK
/* Intense red flash */


[15] Type: BLOCK
/* Letter spacing cinematic text reveal */


[16] Type: BLOCK
/* Shake effect for scares */


[17] Type: BLOCK
/* Slow motion effect */


[18] Type: BLOCK
/* Ritual pulsing effect */


[19] Type: BLOCK
/* Mirror portal effect */


[20] Type: BLOCK
/* Breath fog effect */


[21] Type: BLOCK
/* Reality distortion for fear */


[22] Type: BLOCK
/* Cinematic color shift */


[23] Type: BLOCK
/* Horror blood drip */


[24] Type: BLOCK
/* Pinky emergence */


[25] Type: BLOCK
/* Dialogue box slide in */


[26] Type: BLOCK
/* Intense pursuit effect */


[27] Type: BLOCK
/* ignore */


[28] Type: BLOCK
/**
         * Create a blood splatter texture using canvas
         */


[29] Type: BLOCK
/* no-op */


[30] Type: BLOCK
/* no-op */


[31] Type: BLOCK
/* ignore when DOM not ready */


[32] Type: BLOCK
/**
         * Summon Pinky directly in front of the player.
         * Sets Pinky to an aggressive/prowl state and shows the fear UI.
         */


[33] Type: BLOCK
/* ignore */


[34] Type: BLOCK
/* ignore property define errors in restrictive environments */


[35] Type: BLOCK
/**
         * Show cinematic black bars (letterbox effect)
         */


[36] Type: BLOCK
/**
         * Hide cinematic black bars
         */


[37] Type: BLOCK
/**
         * Fade to black
         */


[38] Type: BLOCK
/**
         * Fade from black
         */


[39] Type: BLOCK
/**
         * Apply glitch effect temporarily
         */


[40] Type: BLOCK
/**
         * Screen shake effect for scares
         */


[41] Type: BLOCK
/**
         * Red flash effect (jumpscare/danger)
         */


[42] Type: BLOCK
/**
         * Slow motion effect
         */


[43] Type: BLOCK
/**
         * Fear/Reality distortion effect
         */


[44] Type: BLOCK
/**
         * Color shift to desaturate/red tint
         */


[45] Type: BLOCK
/**
         * Intense pursuit effect - combines multiple effects
         */


[46] Type: BLOCK
/**
         * Jumpscare sequence
         */


[47] Type: BLOCK
/**
         * Mirror portal appearance effect
         */


[48] Type: BLOCK
/**
         * Reality warping when Pinky is near
         */


[49] Type: BLOCK
/**
         * Breath fog visual effect (adds an overlay that fades)
         */


[50] Type: BLOCK
/**
         * Dialogue box cinematic text reveal
         */


[51] Type: BLOCK
/* ignore */


[52] Type: BLOCK
/* ignore if player not ready */


[53] Type: BLOCK
/* ignore */


[54] Type: LINE
// NEW: Import DecalGeometry


[55] Type: LINE
// --- Custom cursor logic ---


[56] Type: LINE
// --- Global Game State ---


[57] Type: LINE
// loading, menu, settings, intro, playing, paused, end


[58] Type: LINE
// Peek configuration (tweakable)


[59] Type: LINE
// seconds player must look to trigger a peek


[60] Type: LINE
// seconds before trigger to shimmer/highlight mirror


[61] Type: LINE
// chance a peek will occur once triggerTime reached


[62] Type: LINE
// emissive intensity during shimmer


[63] Type: LINE
// how long Pinky remains visible if not interacted with


[64] Type: LINE
// ms until Pinky disappears after being seen


[65] Type: LINE
// chance peek spawns from nearby corner instead of mirror


[66] Type: LINE
// per-trap cooldown between peeks


[67] Type: LINE
// Helper: pick a corner spawn near the player from collidables (returns THREE.Vector3 or null)


[68] Type: LINE
// pick one of the eight corners of the bounding box


[69] Type: LINE
// ensure the corner is not inside the object (push outwards slightly)


[70] Type: LINE
// floor-level spawn


[71] Type: LINE
// pick the candidate closest to player


[72] Type: LINE
// --- DOM Elements ---


[73] Type: LINE
// --- NEW: Texture Loaders and Helper Functions ---


[74] Type: LINE
// Red blood color


[75] Type: LINE
// Create splatter effect


[76] Type: LINE
// Add drips


[77] Type: LINE
// --- Sound System (Tone.js) ---


[78] Type: LINE
// Robustness: if the Tone.js script reported a load failure, immediately fallback


[79] Type: LINE
// Immediate fallback if script onerror fired


[80] Type: LINE
// Provide no-op scheduling/ramp methods expected by Tone usage


[81] Type: LINE
// Mark as initialized to avoid further retries


[82] Type: LINE
// Otherwise retry a few times (shorter timeout) before falling back


[83] Type: LINE
// Retry every 150ms (shorter)


[84] Type: LINE
// Mark as initialized to avoid further retries


[85] Type: LINE
// START Tone audio context


[86] Type: LINE
// FIX: Ensure AudioContext is started on user gesture (handled by play button)


[87] Type: LINE
// We just define the synths here


[88] Type: LINE
// Show a small HUD indicator when audio is unavailable


[89] Type: LINE
// Find a nearby non-colliding spawn point around origin by sampling offsets.


[90] Type: LINE
// Returns a THREE.Vector3 or null if none found.


[91] Type: LINE
// Save original camera and collider positions


[92] Type: LINE
// Check origin first


[93] Type: LINE
// keep same offset


[94] Type: LINE
// Restore original positions before returning


[95] Type: LINE
// place on floor (y=player.height)


[96] Type: LINE
// Restore originals


[97] Type: LINE
// Restore originals if no safe spot found


[98] Type: LINE
// --- Dialogue System ---


[99] Type: LINE
// Ensure minimum readable duration for auto-hide (clamp to 8s)


[100] Type: LINE
// Auto-hide dialogue after specified time (if > 0)


[101] Type: LINE
// NEW: Message box for item/info messages


[102] Type: LINE
// --- Player Class (NEW MOVEMENT) ---


[103] Type: LINE
// Timer for flashlight flicker effect


[104] Type: LINE
// NEW: Flashlight


[105] Type: LINE
// Brighter, wider


[106] Type: LINE
// Starts off


[107] Type: LINE
// FIX: Check for Enter key during intro and playing states


[108] Type: LINE
// Allow Enter to close message boxes


[109] Type: LINE
// Allow Enter to advance dialogue during gameplay


[110] Type: LINE
// Developer / debug: summon Pinky in front of player


[111] Type: LINE
// Don't need to handle Enter during intro on key up


[112] Type: LINE
// Don't interfere with gameplay key ups


[113] Type: LINE
// RMB


[114] Type: LINE
// LMB


[115] Type: LINE
// RMB


[116] Type: LINE
// LMB


[117] Type: LINE
// 'X' button


[118] Type: LINE
// L3


[119] Type: LINE
// 'B'


[120] Type: LINE
// 'X'


[121] Type: LINE
// LT


[122] Type: LINE
// 'Y' button


[123] Type: LINE
// Prevent holding


[124] Type: LINE
// --- NEW: Traditional Movement Logic ---


[125] Type: LINE
// FIX: Corrected movement directions


[126] Type: LINE
// Apply direction relative to camera


[127] Type: LINE
// Ignore camera pitch


[128] Type: LINE
// Adjust collider for crouch


[129] Type: LINE
// Check X-axis collision


[130] Type: LINE
// Debug: movement blocked by collision on X


[131] Type: LINE
// Check Z-axis collision


[132] Type: LINE
// Debug: movement blocked by collision on Z


[133] Type: LINE
// Sound


[134] Type: LINE
// Gasp


[135] Type: LINE
// Brighter


[136] Type: LINE
// Atmospheric flicker every 20 seconds


[137] Type: LINE
// Reset cycle


[138] Type: LINE
// Add slight intensity variation during flicker window (last 1 second of 20-second cycle)


[139] Type: LINE
// Rapid flicker for 1 second


[140] Type: LINE
// Smooth toggle


[141] Type: LINE
// Show item-specific messages


[142] Type: LINE
// NEW: Speed up AI timer


[143] Type: LINE
// Reduce timer by 30s


[144] Type: LINE
// --- Pinky AI Class (NEW SLOW BURN) ---


[145] Type: LINE
// NEW


[146] Type: LINE
// Start aggressive sooner (30s ambient instead of 120s)


[147] Type: LINE
// Track player fear to trigger earlier


[148] Type: LINE
// Start hiss loop


[149] Type: LINE
// Wait longer if sounds failed


[150] Type: LINE
// keep ambient cadence at 20s


[151] Type: LINE
// Make prowling resume on a consistent 20s cadence to match request


[152] Type: LINE
// Keep prowl duration around 20s so Pinky walks around every ~20s


[153] Type: LINE
// Legacy state


[154] Type: LINE
// Shorter between glimpses


[155] Type: LINE
// Only need 2 glimpses to start prowling


[156] Type: LINE
// Don't catch player if they're hiding


[157] Type: LINE
// Pinky pauses and looks around, then moves on


[158] Type: LINE
// Trigger jumpscare sequence


[159] Type: LINE
// Spawn at a point that is FAR away


[160] Type: LINE
// Make Pinky peek from a mirror trap: appear at the mirror's spawnPoint for a short time.


[161] Type: LINE
// Accept either a mirror object with userData.spawnPoint or a pseudo object with spawnPoint


[162] Type: LINE
// fallback


[163] Type: LINE
// If spawn is null, try to find one near player


[164] Type: LINE
// Clear any existing peek timeout


[165] Type: LINE
// Auto-hide after configured ms if not interacted with


[166] Type: LINE
// small shake before disappearance to add tension


[167] Type: LINE
// --- Game Initialization ---


[168] Type: LINE
// Compute forward vector from camera


[169] Type: LINE
// Place Pinky on the floor at spawn position


[170] Type: LINE
// Force aggressive state


[171] Type: LINE
// Show fear UI same as when Pinky detects player


[172] Type: LINE
// Play a warning sound if available


[173] Type: LINE
// Fog for intro


[174] Type: LINE
// Sounds are initialized on 'Play' click


[175] Type: LINE
// Debug helper: allow pressing 'P' to summon Pinky (also handled inside Player.onKeyDown)


[176] Type: LINE
// Expose debug-friendly view into module-scoped runtime objects.


[177] Type: LINE
// Use a getter so values reflect the latest runtime state from the module scope.


[178] Type: LINE
// --- Intro Scene ---


[179] Type: LINE
// This is bound to the dialogue box click OR Enter key


[180] Type: LINE
// Handle chant input pending


[181] Type: LINE
// Handle normal dialogue advancement


[182] Type: LINE
// This is bound to key presses (Enter, E, or Click)


[183] Type: LINE
// Turn flashlight on for player


[184] Type: LINE
// --- CINEMATIC EFFECTS FUNCTIONS ---


[185] Type: LINE
// Phase 1: Subtle distortion


[186] Type: LINE
// Phase 2: Screen shakes


[187] Type: LINE
// Phase 3: Red tint + glitch


[188] Type: LINE
// Phase 4: Intense everything


[189] Type: LINE
// Audio jumpscare


[190] Type: LINE
// Extreme camera shake


[191] Type: LINE
// Red flash multiple times


[192] Type: LINE
// Glitch


[193] Type: LINE
// Cinematic sequence


[194] Type: LINE
// Changed position


[195] Type: LINE
// IMPORTANT: Make sure gameState is 'playing' and controls are unlocked for gameplay


[196] Type: LINE
// Try to ensure pointer lock and controls are unlocked for immediate input


[197] Type: LINE
// Debug: log player spawn position and whether the player collider intersects any collidable immediately after spawn


[198] Type: LINE
// Attempt to find a nearby safe spot and teleport player there


[199] Type: LINE
// Show dialogue but don't block movement


[200] Type: LINE
// Show objectives message after a delay


[201] Type: LINE
// --- Level Building (NEW MAZE) ---


[202] Type: LINE
// NEW: Wet Floor


[203] Type: LINE
// Reflective


[204] Type: LINE
// High metalness for reflection


[205] Type: LINE
// Moldy green


[206] Type: LINE
// --- HUB (Start Area, 10x10) ---


[207] Type: LINE
// This is where the player starts *after* the shift


[208] Type: LINE
// Back wall


[209] Type: LINE
// Add visible stalls/hiding near the start area so player can hide quickly


[210] Type: LINE
// --- ESCAPE OBJECTS - Now Randomized in Maze ---


[211] Type: LINE
// Define random exit positions (moved into maze instead of hub)


[212] Type: LINE
// Shuffle exit positions


[213] Type: LINE
// Create Door


[214] Type: LINE
// Create Window


[215] Type: LINE
// Add a framed border to make the window exit visible


[216] Type: LINE
// Create Sewer


[217] Type: LINE
// --- MAZE (40x40 area - TIGHTER, more claustrophobic) ---


[218] Type: LINE
// Outer Walls (Reduced size for claustrophobic feel)


[219] Type: LINE
// Maze Internals - TIGHTER spacing for claustrophobic feeling


[220] Type: LINE
// Add Stalls/Hiding - RELOCATED positions (in tighter maze)


[221] Type: LINE
// Add Lockers/Hiding - RELOCATED positions (in tighter maze)


[222] Type: LINE
// --- Add Mirrors at Hallway Ends (for atmosphere and reflection) ---


[223] Type: LINE
// Left side


[224] Type: LINE
// Right side


[225] Type: LINE
// Back dead end


[226] Type: LINE
// Front corridor


[227] Type: LINE
// NEW: Add MORE Lethal Mirror Traps (increased danger)


[228] Type: LINE
// Front far


[229] Type: LINE
// Back corner


[230] Type: LINE
// Mid corridor


[231] Type: LINE
// Left mid


[232] Type: LINE
// --- Add Sinks with Dripping Water ---


[233] Type: LINE
// NEW: Add Atmosphere (Bloodstains & Windows)


[234] Type: LINE
// High windows with light


[235] Type: LINE
// Collidable so AI pathing sees it


[236] Type: LINE
// Make lethal mirrors visually identical to regular mirrors so they blend in


[237] Type: LINE
// NEW: High window with "god rays"


[238] Type: LINE
// Simple "god ray"


[239] Type: LINE
// Sink basin


[240] Type: LINE
// Sink legs


[241] Type: LINE
// Faucet


[242] Type: LINE
// Dripping water sound effect - play every 2-4 seconds


[243] Type: LINE
// Start dripping


[244] Type: LINE
// --- Game Loop ---


[245] Type: LINE
// Check for interactable


[246] Type: LINE
// Check for mirror


[247] Type: LINE
// Detect if the player is directly looking at Pinky's mesh (or any descendant)


[248] Type: LINE
// Stop raycasting if we've found the closest interactable and a mirror


[249] Type: LINE
// Track per-mirror look timers: if player looks directly at a lethal mirror (within flashlight range) for 3s, trigger a peek


[250] Type: LINE
// use flashlight distance if available


[251] Type: LINE
// distance from player to trap face


[252] Type: LINE
// Simple visibility check: raycast center of screen to see if the mirror is hit


[253] Type: LINE
// align height


[254] Type: LINE
// subtle shimmer to telegraph peek when approaching 2s


[255] Type: LINE
// shimmer when approaching the trigger threshold


[256] Type: LINE
// stronger emissive pulse to telegraph the peek


[257] Type: LINE
// trigger probabilistic Pinky peek from this trap


[258] Type: LINE
// probabilistic roll


[259] Type: LINE
// maybe peek from a corner instead


[260] Type: LINE
// build a small pseudo-trap object with spawnPoint


[261] Type: LINE
// failed the probability roll; small cooldown to avoid immediate retrigger


[262] Type: LINE
// --- Mirror Logic ---


[263] Type: LINE
// --- Lethal Mirror Trap Logic ---


[264] Type: LINE
// NEW: Visual/Audio warning


[265] Type: LINE
// (peek triggering is handled by per-trap look-timers below)


[266] Type: LINE
// If player directly looks at Pinky while he is peeking, make him disappear within 2s


[267] Type: LINE
// When player sees Pinky, make him disappear within configured ms but add a brief shake just before


[268] Type: LINE
// Reset timers for mirrors not being looked at


[269] Type: LINE
// --- Item/Door Logic ---


[270] Type: LINE
// --- Window & State Management ---


[271] Type: LINE
// Don't auto-pause when pointer lock is lost; show a small prompt instead


[272] Type: LINE
// Defensive fallback: ensure keyboard movement remains enabled even when pointer lock is not active


[273] Type: LINE
// Do not request pointer lock automatically; require user click.


[274] Type: LINE
// Pointer lock requests must come from user gestures in many browsers.


[275] Type: LINE
// Defensive fallback: ensure player controls unlocked so keyboard movement works even without pointer lock


[276] Type: LINE
// Cinematic effects


[277] Type: LINE
// Special mirror jumpscare


[278] Type: LINE
// Cinematic escape sequence


[279] Type: LINE
// --- Gamepad Detection ---


[280] Type: LINE
// --- Menu Button Listeners ---


[281] Type: LINE
// FIX: Start audio context on first click


[282] Type: LINE
// Initialize sounds *after* context is running


[283] Type: LINE
// Failsafe if Tone was already running


[284] Type: LINE
// --- Start Init ---


[285] Type: LINE
// Start the game initialization process
