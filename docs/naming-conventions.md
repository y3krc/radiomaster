# Naming Conventions

How the Y3K RC sounds are named, so they're easy to find and assign on the radio. The live list of sounds is in [`../sounds/inventory.md`](../sounds/inventory.md); this file describes the rules.

## The constraint

EdgeTX shows a `.wav` in the Special/Global Function file picker only if its name is **≤6 characters** (plus `.wav`). Longer filenames exist on disk but are invisible to the trigger UI.

## The `z`-prefix system

All custom sounds start with `z`. EdgeTX sorts filenames alphabetically and its own files start earlier in the alphabet (`0.wav`, `1.wav`, … `hello.wav`, … `telemok.wav`), so a leading `z` clusters every custom sound at the **bottom** of the picker — one scroll and you're at your stuff.

Format: `z` + 5 characters describing the sound — **6 total** (EdgeTX's hard limit for picker visibility). Aim for 6; fall back to 5 only when there's no meaningful 6th character (don't pad with filler).

## Within the z-block

Where possible, related sounds share a 2nd letter so they sub-cluster:

| Prefix | Category | Examples |
|---|---|---|
| `zc*` | Crawlers | `zcrolo` |
| `zh*` | Hit the trail / hookups | `zhttrl` |
| `zj*` | Josiah callouts | `zjolst` |
| `zl*` | Let's go / low gear | `zletg1`, `zlgsrc`, `zlezzr` |
| `zn*` | Norcal / need a tow | `znrchb`, `znedtw` |
| `zo*` | Orion callouts | `zorion` |
| `zp*` | Power events (on/off/inactivity) | `zpwron`, `zpd10m`, `zponht` |
| `zr*` | Roll out / radio master | `zrlout`, `zrmyk1` |
| `zs*` | Save / spool / steep | `zsavem`, `zspoin`, `zsteep` |
| `zt*` | Tow hook | `ztwhkr` |
| `zu*` | You got / unmanned | `zugott`, `zunmna` |
| `zy*` | Y3K branding variants | `zy3aim`, `zy3lg1`, `zy3krm` |

When adding a sound, place it under an existing category prefix where it fits; otherwise pick a new, mnemonic 2nd letter.

## System sound overrides

Files placed in `SOUNDS/en/SYSTEM/` replace EdgeTX's built-in event sounds. The filenames must match **exactly** (so these are not z-named):

| System filename | Plays when |
|---|---|
| `hello.wav` | Radio startup (after switch checks) |
| `inactiv.wav` | Inactivity timeout (set in Radio Setup) |
| `bye.wav` | Radio shutdown |

## Audio format

Every sound must be:

- **Codec**: PCM uncompressed
- **Bit depth**: 16-bit signed
- **Channels**: mono
- **Sample rate**: 32000 Hz

EdgeTX silently skips anything off-spec (no error, just no sound).

Check a file: `ffprobe -hide_banner file.wav`

Convert one: `ffmpeg -i input.mp3 -ar 32000 -ac 1 -sample_fmt s16 output.wav`
