# RadioMaster · Y3K RC

Custom [EdgeTX](https://edgetx.org/) content for [RadioMaster](https://www.radiomasterrc.com/) radios in Y3K RC livery — a **universal voice-prompt sound pack** plus **per-controller model configs**. All sounds are my own; shared freely.

## What's here

```
sounds/                  Universal Y3K RC voice prompts — work on ANY RadioMaster + EdgeTX radio
  inventory.md           The sound list (short name ↔ friendly name)
  naming-conventions.md  The z-prefix naming system + audio spec
models/                  Per-controller model configs (hardware-specific)
  mt12/                  RadioMaster MT12
```

**Why the split?** A sound is just a `.wav` — it plays the same on any RadioMaster radio, so the sound pack is **universal**. Model files encode a radio's switches, mixes, and channels, so they're **specific to a controller**.

## Use the sounds (any RadioMaster radio)

1. Set up an EdgeTX SD card with [EdgeTX Buddy](https://buddy.edgetx.org/).
2. Copy `sounds/*.wav` into your card's `SOUNDS/en/`.
3. Assign them via Special/Global Functions — they all start with `z`, so they cluster at the bottom of the picker. See [`sounds/naming-conventions.md`](sounds/naming-conventions.md).

Every sound is EdgeTX-spec: **PCM 16-bit mono 32 kHz** (EdgeTX silently skips anything off-spec).

## Use a model (your specific controller)

Model files are per-radio. Grab yours from `models/<controller>/`:

1. Copy the `.yml` into your card's `BACKUP/`.
2. On the radio, restore it from the model-select menu (safer than dropping straight into `MODELS/`).

Currently: **[`models/mt12/`](models/mt12/)** (RadioMaster MT12). More controllers as I set them up.

## Pick & choose

Want just one crawl sound or a single model? Browse and grab individual files. Or take the lot: green **Code → Download ZIP**.

---

Part of **Y3K RC** · **Y3K Lab** — https://y3klab.com
