# RadioMaster Pocket — models

Model configs for the [RadioMaster Pocket](https://www.radiomasterrc.com/) (internal **ELRS**) running EdgeTX 2.12.2.

| File | Model | Notes |
|---|---|---|
| `model00.yml` | Y3Kradio | Main radio profile / template |
| `model01.yml` | FPV DRONE | |
| `model02.yml` | DELTA | Delta-wing |
| `model03.yml` | HELI | |
| `model04.yml` | SuperSPrnt | |
| `model05.yml` | AIR | |
| `model06.yml` | **Titan24** | Dual-stick 4WS crawler w/ the **[Crab Fader](https://radiomaster.y3krc.com/crab-fader/)** — front steer + throttle on the right stick, rear steer + hold-position crab stance on the left |

## Install

1. Copy the `.yml` you want into your SD card's `BACKUP/`.
2. On the radio: model-select menu → restore from backup.

> These are **Pocket-specific** (switch map, channel setup) — they won't map cleanly to other RadioMaster radios. The [sounds](../../sounds/) are universal, though.

**Binding:** the Pocket's internal ELRS module keeps bind data in module flash, so bind data isn't stored in the model file — these `.yml` are bind-phrase-free, and you'll bind your own receivers via the ELRS Lua tool.
