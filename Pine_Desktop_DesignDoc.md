# DESIGN DOC — "PINE.OS"
### A diegetic desktop-exploration minigame for *Pokémon: Shima 5e*
**Build target:** single self-contained web artifact (HTML/CSS/JS or React), runnable in a Claude artifact or served locally for the table. Drop this whole file into a Claude Code session as the build brief.

---

## 0. ONE-PARAGRAPH PITCH

The players have Dr. Amelia Pine's login credentials and have used them before. This session they reach her machine from a **different location** — not the Starhaven terminal they remember, but a **personal desktop** that lives somewhere else and has things the work terminal never did. It presents as a full retro-modern operating system: wallpaper, icons, draggable windows, a file browser, a mail client, an image viewer, a notes app, a music player. The players explore at their own pace. There is **no fail-state, no countdown** — the tension comes from a single slow, creeping fact: **someone else is logged into this account at the same time they are**, and over the minutes they spend inside, that someone *does things* — a file appears, a window they didn't open flickers, the cursor isn't always theirs. The desktop's documents resolve three braided discoveries: **where Amelia is now** (Blackthorn Manor), **who Aurora is** (her sister, an amnesiac, and the person all of this is secretly *for*), and **the experience-sharing research** that ties the science to the heartbreak and seeds the Exp. Share side quest.

---

## 1. RETCON & CONTINUITY (read first)

This rebuilds an earlier prop. Reconcile, don't contradict:

- The players previously accessed a **work terminal** (Starhaven Biolabs) and read "the Pine cache" (eight email threads — see `The_Pine_Cache.md`, the canonical source for that correspondence). That still happened.
- **This** machine is a **separate, personal device** at a **second location**. In-fiction, that's why there's new material: this is her private desktop, not the monitored work box. Anything that feels "new" is new because *they've never been on this machine before.*
- Small, deliberate consequence to flag to the GM: logging in here is riskier than the work terminal, because **this account is being actively watched/used by someone else now.** The party leaves a footprint. That footprint is a future hook, not a this-session punishment.
- **"Aurora" reconciliation:** earlier notes floated *"Aurora Drake"* as a pseudonym Pine uses later for desert-crisis propaganda. New canon: **Aurora Pine is Amelia's real sister.** Reconcile by making the future alias an *homage* — when Amelia later writes as "Aurora Drake," she is borrowing her lost sister's name. The desktop should plant Aurora-as-sister clearly; the alias payoff is for much later and need not appear here (optional Easter egg only).

---

## 2. DIEGETIC FRAME — WHOSE MACHINE, WHERE

- **Device:** a personal desktop workstation, Shiman consumer-grade, ether-powered (idle "ether draw" indicator in the taskbar; see §6 flavor).
- **OS name:** invent a Shiman consumer OS brand — suggested **"Lumen OS"** (ties to the setting's light/ether motif; the Blackthorn motto *Knowledge Illuminates the Path* makes "Lumen" quietly resonant if the machine turns out to be Blackthorn-supplied — GM's call).
- **Where the machine physically is (GM truth, discoverable in-fiction):** the desktop is **at Blackthorn Manor** — Amelia has been installed there (guest? prisoner-collaborator? both?), in the manor's quieter quarters. The players don't know they're "calling into" the manor until the environmental clues accrue. This is the session's central reveal: *we found out where she went.*
- **The other user (GM truth):** a second party is in the account. Leave their identity unfixed in the build (GM-configurable). Candidates the art/text should keep *plausible*: Helena Blackthorn (archives curator, inner circle — the most likely "co-user" of a manor machine); a Scepter cleaner; or something the Whispering-Shadow thread implies. The build presents *behavior*, never identity.

---

## 3. CORE LOOP & TONE

Calm archive exploration with ambient dread. The player:
1. Logs in (credentials pre-filled or one-click — they "have" them).
2. Lands on a desktop and pokes around: opens folders, reads files, views images, plays a track, reads mail.
3. Over real elapsed time and/or per-file-opened **progress**, the **co-user events** fire (§5) — small, escalating, never lethal.
4. Assembles the three discovery threads (§4) at their own pace.
5. Can log off whenever; state persists (§7) so a table can return next session and the co-user has "moved things."

**Tone dial:** think *abandoned-but-warm*. Family photos next to lab data. A sister's get-well card next to a redacted research log. The horror is intimacy, not jump-scares.

---

## 4. THE THREE DISCOVERY THREADS (content design)

Distribute these across folders/apps so each is *assembled*, not handed over. Mundane filler (§6) is the camouflage.

### THREAD A — WHERE AMELIA IS (→ Blackthorn Manor)
The environmental-evidence thread. No single file says "I'm at Blackthorn Manor"; the players *triangulate* it. Seed these:
- **Photos** (Image Viewer) with manor-specific backdrops drawn from canon: tall arched **library** windows with mismatched replacement panes; the **observatory tower** with its patina-green copper roof and domed retractable ceiling; wild **thorn-hedge gardens**; a wrought-iron gate sigil — **a thorned branch beneath a single star.** A player who has been to the manor (or read about House Blackthorn) recognizes it.
- A **calendar/notes** entry referencing being "at the house on the promontory," "the salt ruins the windows," "H. wants the west wing left alone" (Helena; the abandoned western wing).
- A **map image** or pinned note with a coastline matching the **northern Libra Coast near the southeastern Florinex border**, Silverpeak foothills descending to sea.
- A mail draft to an unknown recipient: *"They've given me the old tower study to work in. E. uses it when he's here. I try not to be here when he is."* (E. = Elias/Nero — never spelled out.)
- The clincher (optional, gated behind thoroughness): a photo of a **library door lintel** carved with *Knowledge Illuminates the Path* — the Blackthorn motto, unmistakable to anyone who's read the house.

**Payoff:** the party learns Amelia Pine is alive and embedded at Blackthorn Manor — a place several other campaign threads already point to (Joey's riddle; the noble-house network). It converts "Pine vanished" into "Pine is *there*, and so is everything else."

### THREAD B — AURORA (the sister, the amnesia, the heart of it)
The emotional spine. This is what all of Amelia's villainy is secretly *for*.
- **Family photos:** two girls, then two women — Amelia and **Aurora Pine**. Aurora younger, brighter, a field-naturalist type (she should read as someone who loved Pokémon directly, foil to Amelia the lab scientist).
- A **get-well / care thread**: Aurora is in some kind of **long-term care** with profound **memory loss** — she doesn't reliably know Amelia. Notes in Amelia's voice that are unbearably tender and increasingly obsessive: *"She asked who I was again today. I told her I was her sister. She said 'I always wanted a sister.' I left before she saw my face."*
- **The investigation folder** (`/Aurora/` or disguised): Amelia's private, methodical hunt for **how Aurora lost her memory.** This is the hinge that connects B to C. It should read like a scientist refusing to accept "we don't know." Medical records hitting walls; a timeline of Aurora's last lucid months; a recurring redacted event Amelia keeps circling — **something happened during an experience-sharing trial Aurora took part in.**
- Implied tragedy: Amelia joined Scepter / went dark **not for ideology but for access** — to resources, forbidden research, and corruption science that might explain or *reverse* what happened to Aurora. (Keep this subtext, not stated outright. A sharp table infers it. It retroactively recolors the whole Pine Cache.)

**Payoff:** Amelia Pine becomes tragic and legible. The party now holds leverage *and* a moral complication — she is a villain with a reason a paladin would hesitate over.

### THREAD C — EXPERIENCE-SHARING RESEARCH (→ Exp. Share side quest)
The science that braids A-location and B-heartbreak into a questable mechanic.
- Research notes (Notes app + a `/research/` folder) on a program to let **a human and a Pokémon "share experiences"** — sensation, memory, learned skill, *lived time* — across the trainer-Pokémon bond. In-world this is the **origin/lore of the Exp. Share item.** Frame it as ether-mediated: the shared **mauri**/experience flows along an attuned link (this also rhymes with Mystauran *whakawhanaungatanga*/*mauri* if you want a cross-culture thread — optional).
- The science is **dual-edged**, and the notes know it: sharing experience can *teach* (the benign Exp. Share function — a partner gains what it didn't directly earn) but pushed too far it can **bleed or displace** experience — i.e., **memory can move, and memory can be lost.** This is the quiet gut-punch link to Thread B: *Aurora may have lost her memories into a Pokémon, or had them overwritten, during an early experience-sharing trial.*
- Seed **side-quest hooks** explicitly in the files: an early prototype device's location; a test subject's partner Pokémon that "still carries something that isn't its own"; a colleague who walked away in protest (a potential quest-giver/ally); a warning note: *"The Share is not a teaching tool. It is a door. Doors swing both ways."* (Echoes the shadow-corruption "door-work" language from the Pine Cache — same author-brain, deliberate.)

**Payoff:** the players leave with a thread they can *pull into a real side quest* — recover/understand the experience-sharing tech, decide what to do about it, and possibly find a route to Aurora's memories. The Exp. Share item gains a haunted backstory.

---

## 5. THE CO-USER (the "someone else is here" system)

The replacement for a breach-clock: not a threat, an *uncanny presence.* Drive it off a simple **suspicion/elapsed-progress meter** that the player never sees as a number. Tie ticks to time-in-session and files-opened. As it rises, fire escalating events from a tiered pool. **Nothing ever blocks or punishes the player** — events are atmospheric and informational.

**Tier 1 (subtle):**
- Taskbar shows a second active session: **"2 users signed in."**
- A "last active: just now" stamp that isn't the player's activity.
- The music player starts/stops a track on its own once.

**Tier 2 (noticeable):**
- A folder the player already viewed now has **+1 file** that wasn't there.
- A window opens or closes on its own (e.g., the Image Viewer flicks to a photo — *the player gets a free clue this way*; the co-user is "looking at" the Aurora photos too).
- A mail arrives in real time into the inbox, from an internal `.sec` address, one line: *"Are you on the personal box right now?"*

**Tier 3 (direct, still non-hostile):**
- A **chat/IM window** pops: someone types to "Amelia," assuming the player is her. Short, deniable lines. The player *can* type back (free-text or canned options) — and the table's choice of how to impersonate Pine is great drama. The co-user never quite catches on this session (consequence deferred).
- A document **starts deleting itself** — and **stops halfway** (the co-user thinks better of it, or is interrupted). The half-deleted file is *more* revealing for being interrupted.
- Final beat (optional capstone): a single line types into an open notes window, not by the player — *"who is this"* — then the second session drops to **"1 user signed in."** They were noticed. Nothing else happens. Let it sit.

**GM config:** expose toggles for co-user identity hints, event frequency, and whether the IM is interactive. Default to creepy-minimal.

---

## 6. DESKTOP CONTENTS (the full object list)

Build a believable machine. **Camouflage ratio:** for every plot file, 2–3 mundane ones. Mundane files reward curiosity with *character*, not clues.

**Desktop icons / apps:**
- **Files** (folder browser) — the spine.
- **Mail** (`a.pine` personal account — distinct from the work `.lib` address; suggest `amelia.pine@home.net`).
- **Image Viewer** — photos (the richest Thread-A and Thread-B delivery).
- **Notes** — research fragments (Thread C), to-do lists, a grief-journal that's the emotional core of Thread B.
- **Music** — a small playlist; one track is the co-user's tell (§5); track names can carry mood (a song that was "Aurora's favorite").
- **Ether Monitor** (setting flavor) — a little system widget showing the machine's ether draw; idly logs **anomalous resonance spikes** with no source (the build can leave this unexplained — it's the machine sensing *something*; optionally the party's Orb).
- **Recycle/Trash** — half-deleted things; recover for bonus texture.
- **Settings** — wallpaper (a photo of the sisters, optionally), the "2 users" indicator surfaces here too.

**Folder tree (suggested):**
```
~/Desktop
├── Files/
│   ├── Work/                ← dull cover: grant forms, expense reports that don't quite add up, meeting notes
│   ├── Research/
│   │   ├── shared-exp/       ← THREAD C: experience-sharing notes, the "door swings both ways" warning, side-quest seeds
│   │   └── [redacted].enc    ← locked; search-returns-a-hit-but-won't-open (future content gate)
│   ├── Aurora/               ← THREAD B: care thread, the memory-loss investigation, the timeline, the redacted trial
│   ├── Photos/               ← THREADS A & B: manor backdrops + family photos (Image Viewer reads these)
│   ├── House/                ← THREAD A: the "old tower study," "west wing left alone," coastline map, the motto lintel photo
│   └── Personal/             ← grief journal, an unsent letter, a playlist note, mundane life
├── Mail/                     ← personal inbox: one real-time co-user mail (§5), a few mundane, one tender draft to Aurora's carers
└── Trash/                    ← a half-deleted photo; a discarded draft resignation (callback to Pine Cache)
```

**Mundane-file ideas (texture, no plot):** a recipe; a furious half-written complaint to a utility company about ether-billing; a wishlist; vacation photos from before everything; a budget spreadsheet with a line item quietly labeled "A.'s care — monthly"; a meme-equivalent; an overdue-library-book notice (nice irony at a Blackthorn machine).

---

## 7. TECH & BUILD NOTES (for the Claude Code session)

- **Single self-contained artifact.** No external assets that can't be inlined. If images are needed, generate them as **CSS/SVG mock-photographs** or solid-color "photo" cards with captions, OR leave labeled image *placeholders* the GM can swap (the manor backdrops can be evocative SVG rather than real art — keep it diegetic-stylized, not realistic).
- **Windowing:** draggable, focus-able, minimizable windows; a taskbar; a clock; the "users signed in" indicator. Classic desktop-metaphor. Mobile-friendly fallback: tap-to-open full-screen "windows."
- **State / persistence:** use the artifact persistent-storage API (`window.storage`) so a table can **return across sessions** and find the co-user has altered things. Persist: which files have been read, the suspicion tier reached, any IM exchange, and which "co-user mutations" have fired (so they don't repeat / so they *advance* next login). **No browser localStorage** (unsupported in-artifact).
- **GM config object** at top of the code: `{ coUserIdentityHints, eventFrequency, imInteractive, startingTier, showEtherSpikes, unlockEncFiles }`. One place for you to tune the whole experience before a session.
- **No real network calls.** The "Mail" and "IM" are local fiction.
- **Aesthetic:** your established house style — near-black surfaces (#1a1a1a / #2a2a2a), **orange accent (#ffa500)** as the system/alert color, monospace for system chrome, a warmer serif/sans for the human documents (the grief journal should *look* different from the lab notes — typography as characterization). The ether motif = thin cyan/violet glow accents used sparingly against the orange.
- **Reading flow:** files open in their app window with readable typography; long docs scroll; redactions render as solid blocks `████` (never selectable-to-reveal — redaction is permanent for now).
- **Audio (optional, off by default):** low room-hum loop; soft key clicks; a single soft chime when a co-user event fires. Respect an audio toggle.

---

## 8. WHAT THE PLAYERS SHOULD LEAVE WITH

1. **A place:** Amelia Pine is alive and at **Blackthorn Manor** — converging with the campaign's existing Blackthorn threads.
2. **A person:** **Aurora Pine**, the amnesiac sister — the human reason behind Amelia's choices, and a moral complication for any party that catches her.
3. **A quest:** the **experience-sharing / Exp. Share** research — a pullable side quest with an ally-in-protest, a prototype to find, and a possible (dangerous) route to restoring Aurora's memories.
4. **A feeling:** they were not alone in there. Someone watched them read, and may now wonder who was using Amelia's account. That unease is the price of admission and the seed of the next complication.

---

## 9. STRETCH / OPTIONAL

- **Returning-visit design:** on a second login (persisted), open cold with *"Files changed since your last session: 3"* and let the co-user's between-session edits be the new content — a clean way to feed this out across multiple game sessions.
- **The interactive IM** as a full small scene: 4–6 exchanges where the table improvises being Amelia; track a hidden "cover intact?" flag for the GM.
- **The Ether Monitor** as a quiet puzzle: the resonance spikes correlate with which folder is open (it spikes hardest on the `shared-exp` research) — a player who notices gets a free thematic hint that the experience-sharing tech is *ether-active right now, in this house.*
- **Aurora's playlist** track that, if played during a co-user event, makes the co-user **pause** (they're listening too) — a tiny, wordless suggestion that the other user has feelings about Aurora as well. (Who would? Save it.)
```
```
**Source-of-truth cross-refs for the builder:** `The_Pine_Cache.md` (prior correspondence & tone), `Blackthorn_Manor.md` (every manor visual detail used in Thread A), `House_Blackthorn.md` (Helena, the motto, the tower study, the west wing). Keep all faction names and `.fed/.lib/.sec/.net` domain conventions consistent with those files.
```

---

## 10. BUILD ADDENDUM — what the current `index.html` actually does

The live build (`index.html`) has grown past this brief. Where the two disagree, the build is current. Differences and additions worth a GM's notice:

- **Photos are real image files.** The nine Image-Viewer photos and the wallpaper prints load from `images/` (Firefly-generated, composited). The original SVG mock-photos remain in code as automatic fallbacks if the folder is absent. Generation/compositing prompts are in `Image_Generation_Prompts.md`.

- **Wallpaper.** Three options in Settings: **the two of us** (the sisters dock photo — the default, per the Character Bible's "keeps the photographs as her wallpaper"), **the walk down** (the seagulls photo), and **Lumen** (stock abstract). The co-user can change it back to the sisters mid-session (a Tier-2 event).

- **The IM is now choice-only, not free-text, and is a branching tree.** The player can no longer type — they pick from 2–3 canned replies per node, and the conversation forks extensively (the co-user reads as **Helena / "H."**, the manor co-user). Key branches: a *cover-crack* path (answer wrong and the channel closes, `coverIntact=false`, the second session drops); a passable *passphrase* check — H. asks for "the thing you say when I worry," and **"Slowly, and safely"** (from `notes-from-the-house.txt`) is the correct de-escalating answer; and several lore-leaking branches (the Federation auditors, "E."/Nero's movements, the west wing, the surveyor party). Parenthesised options like *(say nothing)* are silent choices. The tree persists and resumes mid-conversation across logins. `imInteractive:false` still falls back to an un-answerable scroll.

- **Mail has four folders.** Inbox, **Drafts**, **Sent**, Archive(work). Drafts holds the unsent letter to the protester technician (the carrier-quest witness) and two abandoned drafts; Sent holds her side of the carer correspondence plus mundane logistics. A Tier-3 co-user event **appends a line to the technician draft in real time** ("leave him alone. he has paid enough.") — H. knows who that letter is to.

- **Ether Monitor is animated and interactive.** Live dual-waveform (a calm cyan house draw; a violet "second draw — not this device" line appears once suspicion rises). A **TRACE CIRCUIT** button runs a sweep and logs results: the first trace exposes the **west wing's unmetered 9.8u draw** (the ether-bill mystery, now load-bearing — something runs over there); a later trace, once the co-user is active, reveals **a second console on the account reading the same files.** Ambient log ticks run on a timer.

- **New app — Browse.** A small web explorer with a start page of bookmarks and six visitable "sites," each diegetic and lore-flavoured: Coast Ether & Power (enquiry ████-4471 still OPEN), Libra University (Yucca's cohort; Pine "on extended leave"), Starhaven Biolabs (the "report mail that seems unlike a colleague" notice), the **Promontory Noticeboard** (villagers gossiping about the tower lights — the richest Thread-A reinforcement), the Coast Herald (the desert corridor, the estate audits), and Reedside Continuing Care (Aurora's facility — the aviary, the "kind visitor," a family portal that logs your sign-in attempt). Browsing history persists; a Tier-2 co-user event injects **ghost history entries** (a visit to Reedside and an attempt at a `████.sec/ledger` address that won't resolve).

- **More co-user (second-session) events,** spread across all three tiers: the ether circuit gaining a second draw signature; the co-user playing Aurora's track; ghost browsing history; the wallpaper being changed back; the draft line appended; and a failed decryption spike on the sealed `redacted-trial.enc` from the other console.

- **Login goes fullscreen** (best-effort `requestFullscreen` on sign-in).

These extend the same design spine — calm archive exploration, ambient dread, the co-user as presence-not-threat. Nothing here introduces a fail state.
```
