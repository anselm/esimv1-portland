# esimv1-portland

Project-specific orientation only. House policy (devlog, git, UX, writing, deploy) comes from the
harness and is not repeated here.

## What this is

Portland, Oregon after a magnitude 9 Cascadia earthquake, as an esimv1 scenario: ground motion, buildings, bridges, power, fuel tanks, hospitals and the year after.

## Where things are

- One project folder with its record inside it.
- The project's manifest is frozen: a change to the source manifest reaches it only at `esim project update
  anselm/portland-cascadia --manifest scenarios/esimv1-portland/manifests/q1-portland-cascadia.js` and a rerun of
  every variant. Last done on 2026-11-28 for the move to the data warehouse; all ten runs came out with the same
  log digests as before. (A note here used to say to ask first; it dated from the night of 12 November and the
  project was rerun on the 13th and 14th.)
- Since 2026-11-28 the maps' roads, bridge lines and place names come from the data warehouse (`data` in the
  manifest; needs engine 0.4.0). Railway bridges are no longer drawn as lines, because a roads product has no
  railways. The record folder under `portland-cascadia/data/events/` is unchanged and still in this repository.
- A Portland run writes a 1.4 GB `snapshots.json`; the 15 GB of runs on canada1 are not in git.
- On canada1 the working clone is `~/projects/2026/earth-simulator-1/scenarios/esimv1-portland`, linked into the hub's
  `projects/anselm/`. History and facts before 22 November 2026: `anselm/esimv1`, `CLAUDE.md` and `devlog/`.

