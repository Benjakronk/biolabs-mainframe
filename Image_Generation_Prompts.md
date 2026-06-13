# Image Generation Prompts — Pine Desktop Photos

Replacements for the nine SVG mock-photos in `index.html` (Image Viewer shows them at 3:2 landscape — generate everything at 3:2). All prompts are purely descriptive, no setting names.

Workflow: generate the **environment** in Adobe Firefly, then (for the two character shots) **composite** the character images in ChatGPT using the composition prompt. Firefly is unreliable with lettering — where an image contains text, fix it in the compositing pass with the note given.

---

## Set 1 — Environments (Adobe Firefly)

**1. Sun-bleached dock** *(for `two-of-us.img` — the sisters photo, also the desktop wallpaper)*
> Old weathered wooden dock over a calm sea, bright hazy summer afternoon, sun-bleached planks, simple wooden railing with posts, pale blue-grey water to the horizon, vintage 35mm family snapshot, warm faded colors, slight overexposure, empty scene, eye-level view.

**2. River reeds** *(for `aurora-field.img` — the young woman doing fieldwork)*
> Shallow river edge thick with tall green reeds, soft morning light, gentle ripples, muddy bank, lush greens, documentary nature photo, slightly faded film look, open space at center frame for a standing figure, eye-level.

**3. Neglected grand library** *(`manor-library.img`)*
> Vast double-height private library, dark wood shelves, iron spiral staircase, rolling brass ladder on rails, tall arched windows where a few panes are mismatched cheaper glass, shafts of dusty light, whole sections of shelf standing empty, no people, desaturated, moody natural light.

**4. Stone tower from below** *(`tower-from-below.img`)*
> Looking up from ground level at a five-storey old stone observation tower against a grey overcast sky, peaked copper roof weathered to green patina, domed top with a retractable panel, all windows dark except one upper window glowing warm and low, coastal setting, gloomy, desaturated, photographic.

**5. Rusted estate gate** *(`gate.img`)*
> Close-up photo of a rusted wrought-iron estate gate hanging slightly askew on its hinges, ornate ironwork centerpiece of a thorned branch beneath a single five-pointed star, behind the gate out of focus: tangled hedges taller than a person and a dark weathered grey limestone facade, overcast light, desaturated, shallow depth of field.

**6. Carved door lintel** *(`lintel.img` — contains text, see composite note)*
> Interior photo of carved capital letters above a heavy old wooden door, worn stone with traces of lost gilding in the letters, lit by a single shaft of daylight from a tall arched window, drifting dust, dark surroundings, moody and quiet.

**7. Coastal survey map** *(`coast-survey.img` — contains text, see composite note)*
> Top-down photo of a weathered vintage coastal survey map, hand-drawn ink, a dark rocky promontory jutting into the sea, foothills descending to the coastline, a dashed boundary line to the east, aged paper with fold creases, soft window light.

**8. Gulls on a railing** *(`gulls.img`)*
> Six seagulls perched in a row along a weathered metal railing, flat grey sky and sea behind, overcast coastal light, plain candid photo taken from a window, deliberately mundane composition, muted colors.

**9. Tea-ring desk corner** *(`tea-rings.img`)*
> Top-down photo of an old dark wooden desk corner, a stack of worn cloth-bound journals, a cluster of overlapping brown tea-ring stains on the wood like a constellation, warm low lamp light, deep shadows, candid still life.

---

## Set 2 — Composition (ChatGPT image, character refs + environment)

**1. Sisters on the dock** *(env 1 + both character images)*
> Composite the two provided women onto the dock photo, standing mid-ground at the railing, squinting into bright sunlight. The dark-haired serious one stands slightly behind with an arm around the other's shoulders, faint reluctant smile; the other is mid-laugh, holding a small pale round object up in both hands. Match the warm faded vintage grading, soft focus and film grain. Add a thin white photo border with a handwritten pencil caption along the bottom: "Amelia & Aurora — before either of us knew anything".
>
> *Optional childhood variant: render the two as young girls, about ten and seven, keeping the same hair, faces and expressions.*

**2. Woman in the reeds** *(env 2 + the younger woman's image)*
> Place the provided woman knee-deep among the reeds at center frame, in practical field clothes with an open notebook in one hand, caught mid-delight, looking down at the water near her boots. Match the soft green morning light, faded film grading and light grain. Optionally add two or three small indistinct water creatures rippling the surface near her boots.

**3. Lintel text fix** *(env 6, no characters)*
> Clean up the carved inscription so it reads exactly "KNOWLEDGE ILLUMINATES THE PATH" in worn Roman capitals across the stone lintel, weathered and chipped, traces of old gilding in the letter grooves. Change nothing else.

**4. Map annotations** *(env 7, no characters)*
> Add a small hand-drawn ink star at the tip of the promontory and, beside it, two pencilled handwritten words: "the house". Add a faint printed label "Silverpeak foothills" along the hills inland. Change nothing else.

---

**Notes**
- The half-deleted photo in Trash (`untitled-deleted.img`) reuses the sisters image — no separate generation needed.
- The sisters and reeds photos also appear as prints in the default desktop wallpaper; the finals can be swapped in there too.
- Keep all finals at 3:2 (e.g. 1536×1024); the viewer letterboxes anything else.
