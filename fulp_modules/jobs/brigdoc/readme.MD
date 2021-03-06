## Title: Brig Physician

MODULE ID: BRIGDOC

### Description:

Adds the Brig Physician job to the game. This includes all the brig physician clothing, landmark, and gamemode overwrites.

### TG Proc Changes:

- code/modules/jobs/jobs.dm > GLOBAL_LIST_INIT(security_positions, list()
- code/modules/jobs/access.dm > /proc/get_all_accesses()

### TG files changed:

- code/modules/mob/living/carbon/human/species_types/plasmamen.dm > Added brig physician plasmaman outfit.
- code/datums/traits/negative.dm > Added brig physician heirloom.
- code/game/machinery/crew.dm > Added brig physician to the job list datum.

### TG procs overwrites:

- update_overlays() (code/game/objects/items/cards_ids.dm) > Assigns ID Overlays for Fulp jobs.
- sec_hud_set_ID() (code/game/data_huds.dm) > Assigns HUD Overlays for Fulp jobs.

### Additional information:

This adds 100% support for new fulp-exclusive jobs, trying to avoid as much conflicts. For more info on how to (mostly) create a new fulp-exclusive job, contact SgtHunk on the Fulpstation discord.

### Credits:

Skyrat - .md template, Original plasmaman envirosuit sprites (https://github.com/Skyrat-SS13/Skyrat13/pull/933)
HomingPenguins - Armored labcoat sprites
MaltVinegar - HUD/Card sprites
Mithrandalf - Original jumpsuit and beret sprites (https://github.com/TheSwain/Fulpstation/pull/163 || https://github.com/TheSwain/Fulpstation/pull/108)
SgtHunk - Coding
