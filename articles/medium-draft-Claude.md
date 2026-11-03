# Piano House: four MIDI kits, built from rules and checked by script

DRAFT. This article has not been published.

Piano house kits: syncopated piano stabs, offbeat bass, four-on-the-floor drums and seventh and ninth chords at 120 to 126 BPM. The pack holds four kits. Each kit has six roles with two variations each as 8-bar MIDI parts, plus one 32-bar arrangement that places those parts. That is 52 MIDI files you can open in any DAW.

## What is inside

- **Floor Seven**: 124 BPM, A aeolian. Chords: Am7 (2 bars) | Dm7 (2 bars) | G7 (2 bars) | Cmaj7 (2 bars).
- **Brass Lamp**: 122 BPM, F dorian. Chords: Fm9 (2 bars) | Bb9 (2 bars) | Ebmaj7 (2 bars) | C7 (2 bars).
- **Late Lift**: 126 BPM, C ionian. Chords: Cmaj7 (2 bars) | Em7 (2 bars) | Fmaj7 (2 bars) | G7 (2 bars).
- **Riverside**: 120 BPM, E aeolian. Chords: Em9 (2 bars) | Am9 (2 bars) | D9 (2 bars) | Gmaj7 (2 bars).

Roles in every kit: drums, bass, keys, motif, sequence and pad. The motif and the sequence never play together in the arrangement. The last eight bars restate the motif from the first eight, so each arrangement has a beginning, a middle and a return.

## How it was made

A script writes the notes from fixed rules and a seeded random generator, so the same inputs give the same MIDI bytes. Then a separate validator reads every file back and checks the format, the tempo, the note ranges, the polyphony limits, the drum map, and that the two variations of a part differ. A second MIDI parser counts the notes again as a cross-check. The validator also rejects a deliberately broken file and accepts a clean one, so you know it can fail. Result for this build: 52 files checked, 0 errors.

## How to use it

Use the keys part for stabs, the bass and drums for the floor, and the motif as the piano riff.

Use either the combined arrangement or the separate parts. Do not stack the part files on top of the combined file. No program changes are encoded. A conventional GM player will normally use its default piano program for pitched channels unless configured otherwise; compatible GM channel 10 percussion is treated separately. Player behavior may vary.

## What the preview is

Preview is Floor Seven bars 17-32 at 124 BPM, 31.007 seconds, not the 32-bar MIDI. It is a simple synthesized render of the MIDI, made so you can hear the structure. It is preview, not a master. No human listening audition was performed for this build.

## Limits

The files are notes only. They contain no samples, no sound design and no mix. The artwork is an illustration drawn by code. No license is set in the repository yet.

Repository: https://github.com/mizcausevic-dev/piano-house
