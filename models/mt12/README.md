# RadioMaster MT12 — models

Model configs for the [RadioMaster MT12](https://www.radiomasterrc.com/) (internal ELRS) running EdgeTX 2.12.1.

| File | Model | Notes |
|---|---|---|
| `model00.yml` | Tr4ctor | |
| `model01.yml` | CAR3 | |
| `model02.yml` | CAR4 | |
| `model03.yml` | CAR5 | |
| `model04.yml` | Tr4ctor2 | Three drive modes (Trail / Crawl / Climb on SA), speed-sensitive steering, trim-button sound triggers, mode-change voice announcements |
| `model59.yml` | MT12 | |

## Install

1. Copy the `.yml` you want into your SD card's `BACKUP/`.
2. On the radio: model-select menu → restore from backup.

> These are **MT12-specific** (switch map, channel setup) — they won't map cleanly to other RadioMaster radios. The [sounds](../../sounds/) are universal, though.

**ELRS:** bind phrases live in the radio's internal-module flash, not the model file — these `.yml` are bind-phrase-free, so you'll bind your own receivers.
