# The Music World: design notes (not built yet)

Idea from the author, 16 Oct 2026. One chapter becomes a music-themed action RPG world, in the spirit of the "music world" episode of a TV show where the hero gains a core instrument. The **piano** is the core item. The player can play it just for fun, and it is also what lets them *travel* through this chapter.

**Decided (17 Oct 2026): this is Chapter 6.** Its poem is "Communicate", which fits. Its track in the game is already "Shades". Chapter 6 is not built yet; this file is the plan.

## What the author asked for
- A real ARPG feel: dungeons, an overworld, not another small island.
- **6 cities or kingdoms, 3 villages, a forest**, and more around them.
- Everything themed on music; **taming creatures** (with music).
- The piano as the key item, with a **memory quest**: play a tune back in order.
- A music player / "music queue" of the game's own (already started: five embedded tracks, per-chapter).

## What already exists to build on
- **Piano** (Build 18): playable keyboard from the Pixel Piano art, with a Simon-style `pianoGame(seq, callback)`. The callback is where a quest hooks in.
- **Instruments and more** sheet (library: asset_library/music_world): 12 guitars and basses, 3 keytars, 4 drum kits, synth rigs on stands, amps, acoustic guitars, tambourines, pedals, turntable, microphone stands, 6 posters. Good for music shops, stages, concert halls, a battle-of-the-bands arena.
- The **prop system** (Build 18) lets big sprites sit in a scene and be walked behind.
- The **lock/gate engine** from Chapters 4 and 5 (state-driven tiles that open and close) can drive dungeon doors.
- Per-chapter music (a track per kingdom is easy).

## A first sketch, to react to (nothing here is decided)
- **Overworld:** one large map (about 3x the size of a normal island) with six kingdom districts around a central concert hall. Roads between them, a forest in the middle with the villages at its edge.
- **Six kingdoms, one per instrument family:** Strings (guitar and bass), Keys (piano and synth), Drums (rhythm), Winds, Voice (mic and choir), and Electronic (turntables). Each is a themed town with one dungeon.
- **Three villages:** small, quiet, where the quests that explain the world live.
- **The piano's powers:** unlocking "tuning gates" (play the right chord to open a door), calming wild creatures, and crossing gaps (notes make a bridge appear).
- **Taming:** creatures respond to a short melody. Play it back correctly (the memory game) and they follow you; each tamed creature gives a small ability or a collectible.
- **Dungeons:** rhythm and memory rooms, using the same piano game engine, ending in a boss that is a "wrong note" the player has to resolve.
- **The final task:** compose a short tune from notes found in the world; it plays at the end.

## Open questions for the author
1. Which chapter should it be, and what is its poem about?
2. Is combat wanted (an action RPG) or only puzzles and taming?
3. How long should it be compared with the other chapters?
4. Should the six kingdoms be six separate maps with a world map, or one large connected map?
5. What is the piano's story origin (where does the player get it)?


---
## Asset map for Chapter 6 (what each pack is for)
| Need | Asset | Notes |
|---|---|---|
| The six kingdoms (towns) | **Serene Village Revamped** (tiles), **Top-Down Retro Interior** (shops, halls, houses inside) | One town style per instrument family, recoloured per kingdom |
| Instruments as set dressing, stages, shops, a concert hall | **Instruments and more** sheet (guitars, drums, keytars, synths, amps, mic stands, turntable, posters) | Drum kits and synth rigs are big landmarks |
| The forest and the three villages | **Gentle Forest** (jungle and forest tiles and trees) and the **Trees** sheets | Forest as the wild middle between kingdoms |
| Dungeons | **Valley Ruin Asset Pack V0.3** (ruins, rock, cliffs), **Crawling Depths** for a darker one | Rhythm and memory rooms |
| Creatures to tame | **Basic Asset Pack** animals (wolf, sheep, pig, frog, turtle, chicken, boar, porcupine) plus the **Minifolks Forest Animals** | Each answers to a short melody |
| The piano | **Pixel Piano** (already built, with the repeat-the-tune game) | Key item: gate-opening chords, calming creatures, bridges of notes |
| A Kingdom of Strategy | **Pixel chess** (Dani Maccari) | A chess puzzle room or a duel with a king; credit already in the game |
| Stars and magic effects | **nyknck star animation** | Already used in the merge ceremony |
| Music | Chapter 6 track is **Shades**; Americano is the title music; room for a track per kingdom later | |

## Licence notes found while mapping assets
- **Penzilla Design** (licence PDF supplied): mandatory credit "Graphics created by Penzilla Design" in the credits; any edits must be listed in full next to the credit; for a public project a link must be emailed to PenzillaDesign@gmail.com; one purchase covers **one project**; the licence is non-transferable (it belongs to the person who bought it); and, importantly, **§9 forbids using the assets in creating AI or machine-learning datasets or models without explicit permission**. Using the art as game graphics is not that, but because the art is being handled through an AI assistant, the safe step is a one-line email to Penzilla asking for explicit permission, which can be sent together with the project link. It is still not known which supplied pack is Penzilla's.
- **Dani Maccari's chess**: free with attribution, may be edited, may not be redistributed or resold on its own.
- **nyknck's star**: credit "@nyk_nck"; commercial use allowed.
- **Seliel the Shaper** (Gentle Forest, Mana Seed): credit required.

## Open questions (still)
1. Combat or no combat? 2. How long should the chapter be? 3. Six kingdoms as separate maps with a world map, or one large map? 4. How does the player first get the piano?
