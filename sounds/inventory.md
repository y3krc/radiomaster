# Sound Inventory

Current 6-char z-names and their friendly-name counterparts.

The system, prefix grammar, audio spec, and add-a-sound workflow live in [`naming-conventions.md`](naming-conventions.md). This file is the live list that grows over time.

## Inventory

| Short name | Friendly name | Notes |
|---|---|---|
| `zcrolo.wav` | crawlers_roll_out.wav | |
| `zhttrl.wav` | hit_the_trail.wav | |
| `zjolst.wav` | josiah_lost.wav | |
| `zletg1.wav` | trail_expedition_letsgo.wav | |
| `zletg2.wav` | trail_expedition_letsgo_v2.wav | |
| `zletg3.wav` | trail_expedition_letsgo_v3.wav | |
| `zlgsrc.wav` | low_gear_serious_climb.wav | |
| `zlezzr.wav` | lezz_roll.wav | |
| `znrchb.wav` | norcal_hobbies.wav | |
| `znrchc.wav` | norcal_hobbies_crawler.wav | |
| `znrcks.wav` | res_concepts_norcal_rocks.wav | |
| `znedtw.wav` | need_a_tow.wav | |
| `zorion.wav` | orion_jr_do_this.wav | |
| `zpd10m.wav` | power_down_10min_inactivity.wav | Candidate for `inactiv.wav` system override |
| `zpd05m.wav` | power_down_5min_inactivity.wav | |
| `zponht.wav` | power_on_hit_trail.wav | |
| `zpwron.wav` | power_on.wav | Candidate for `hello.wav` system override |
| `zrmyk1.wav` | radio_master_y3k_rc.wav | |
| `zrmyk2.wav` | radio_master_y3k_rc_v2.wav | |
| `zrlout.wav` | trail_expedition_rollout.wav | |
| `zsavem.wav` | save_these_guys.wav | |
| `zspoin.wav` | spooling_in.wav | |
| `zspoot.wav` | spooling_out.wav | |
| `zsteep.wav` | too_steep.wav | |
| `ztwhkr.wav` | tow_hook_retracting.wav | |
| `zugott.wav` | you_got_this.wav | |
| `zunma2.wav` | unmanned_alert_powerdown_v2.wav | |
| `zunmna.wav` | unmanned_alert_powerdown.wav | |
| `zy3aim.wav` | y3k_rc_radio_master_AI_mode.wav | |
| `zy3lg1.wav` | y3k_rc_radio_master_letsgo.wav | |
| `zy3lg2.wav` | y3k_rc_radio_master_letsgo_v2.wav | |
| `zy3lg3.wav` | y3k_rc_radio_master_letsgo_v3.wav | |
| `zy3lg4.wav` | y3k_rc_radio_master_letsgo_v4.wav | |
| `zy3km1.wav` | y3k_rc_radio_master.wav | |
| `zy3krc.wav` | y3k_rc.wav | |
| `zy3krm.wav` | power_on_y3k_rm.wav | |
| `zy3etx.wav` | power_on_y3k_edgetx.wav | |
| `zy3wrm.wav` | power_on_y3k_welcome_rm.wav | |
| `zmcraw.wav` | Crawl mode.mp3 | Mode-change announce: SA1 (mid) → Crawl |
| `zmtral.wav` | Trail mode.mp3 | Mode-change announce: SA0 (up) → Trail |
| `zmclmb.wav` | Climb mode.mp3 | Mode-change announce: SA2 (down) → Climb |

Total: 41 custom sounds.

## System-override candidates

Sounds in this inventory that are candidates for `sdcard/SOUNDS/en/SYSTEM/` (replacing EdgeTX's built-in event sounds):

- `hello.wav` (radio startup): `zy3wrm.wav` or `zpwron.wav`
- `inactiv.wav` (inactivity timeout): `zpd10m.wav` or `zunmna.wav`
- `bye.wav` (radio shutdown): `zhttrl.wav` (as a sign-off)

See [`naming-conventions.md`](naming-conventions.md) for the system-override mechanism details.
