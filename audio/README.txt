PINE.OS — Music app audio
==========================

The Music app ("for the tower") maps each playlist row to a file in THIS folder.
The files in place (spaces are URL-encoded as %20 in index.html's `src` paths):

  Salt Glass.mp3                "Salt Glass"
  The Long Way Down.mp3         "The Long Way Down"
  Reeds.mp3                     "Reeds (A.'s)"  ← the special track (track 3)
  Static off the Water.mp3      "Static off the Water"
  Five Flights of Cold Stone.mp3 "Five Flights of Cold Stone"

Track character (what each should sound like)
---------------------------------------------
1. Salt Glass        Slow, glassy instrumental: lone piano under a high shimmer
                     (bowed / glass-harmonica tones), heavy reverb, no percussion.
                     Cold and still.
2. The Long Way Down Grey folk-ambient with a slow forward pulse — low fingerpicked
                     guitar or muted piano like trudging footsteps. Distant.
3. Reeds (A.'s)      The warm one: intimate, close-mic'd acoustic — gentler and
                     more human than the rest. The co-user "someone is listening"
                     track (Aurora's song). Instrumental, like all five.
4. Static off the    Dark ambient: low drone laced with sea-noise and radio static,
   Water             beatless and unresolved, quietly menacing.
5. Five Flights of   Sparse neoclassical: a repeating figure that climbs and never
   Cold Stone        quite arrives, stone-cold reverb, a sense of weight.

Notes
-----
- Format: MP3 is assumed (widest browser support). To use .ogg/.m4a/.wav,
  change the `src` paths in index.html (const TRACKS).
- Filenames must match the `src` paths in index.html exactly (spaces as %20). If
  you rename a file, update its `src` in const TRACKS to match.
- If a file is ever missing, that row still "plays" visually (no sound) — the game
  and the scripted music events do not break on a missing file.
- These files are NOT in git yet. If you want them version-controlled, `git add`
  them; otherwise they'll just sit alongside the images.
