# J4F-Hand-Tracking-animation-using-MediaPipe
Interactive cat's cradle hand tracking animation
using claude ai
Download and open directly in Chrome or Edge — camera APIs require a local file context, not an iframe.
What's in here:
The app loads three external libs (p5.js, MediaPipe Hands, Camera Utils) and builds everything in one file. 
On load it requests camera access, feeds frames into MediaPipe, and p5 draws each frame with:

  Silhouettes — two-pass glow render of all 21 hand landmarks per hand; cyan tint for left, magenta for right. Raw video never shown.
  Laser strings — five strings connecting matching fingertips (thumb↔thumb, index↔index, etc.). Each string is a 4-layer composite: wide diffuse glow → mid gradient → core line → white fiber. Color cycles cyan→magenta→yellow as hands stretch apart; thickness drops as distance increases.
Particle bursts — when matching fingertips come within ~45px, 28 particles explode outward with trails and a shockwave ring. Each finger gets its own color and a 250ms cooldown so it doesn't spam.
  CRT scanlines — CSS repeating-linear-gradient that slowly scrolls to mimic phosphor refresh.
  HUD overlay — monospace status, hand count, corner brackets, all pointer-events: none so they don't interfere.

One honest caveat: MediaPipe's handedness label is flipped in mirrored display — "Left" in its coordinate space appears on your right side on screen.
