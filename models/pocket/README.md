# RadioMaster Pocket — models

Model configs for the [RadioMaster Pocket](https://www.radiomasterrc.com/) (internal 4-in-1 multiprotocol / CC2500) running EdgeTX 2.12.2.

| File | Model | Notes |
|---|---|---|
| `model00.yml` | Y3Kradio | Main radio profile / template |
| `model01.yml` | FPV DRONE | |
| `model02.yml` | DELTA | Delta-wing |
| `model03.yml` | HELI | |
| `model04.yml` | SuperSPrnt | |
| `model05.yml` | AIR | |

## Install

1. Copy the `.yml` you want into your SD card's `BACKUP/`.
2. On the radio: model-select menu → restore from backup.

> These are **Pocket-specific** (switch map, channel setup) — they won't map cleanly to other RadioMaster radios. The [sounds](../../sounds/) are universal, though.

**Binding:** the Pocket drives its internal 4-in-1 multiprotocol module, so bind data isn't stored in the model file — these `.yml` are bind-phrase-free, and you'll bind your own receivers.
