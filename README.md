# esimv1-portland

Portland, Oregon after a magnitude 9 earthquake on the Cascadia subduction zone: the
shaking, the buildings, the bridges, the power, the fuel tanks along the Willamette, the
hospitals, and the year after. Shown at
[/anselm/portland-cascadia](https://esimv1.exe.xyz/anselm/portland-cascadia).

- `portland-cascadia/` is the project: description, manifest, page, README.
- `portland-cascadia/data/events/portland-cascadia/` is its record: DOGAMI's ground
  layers and loss tables, the county's tank study, the bridge inventory, poles and routes.
  The folder's README names each source and how it was cut.
- `manifests/q1-portland-cascadia.js` is the manifest as written.

The project's README says what is computed, what is arranged, and what is known to be wrong.

## Run it

This is content for [esimv1](https://github.com/anselm/esimv1): the description, the
manifest, the record the model is read against, and the page. It holds no code. With a
built [esimv1-core](https://github.com/anselm/esimv1-core) (0.3.0 or newer):

```
ESIM_ROOT=/path/to/esimv1-core /path/to/esimv1-core/target/release/esim project run ./<project folder> --variant <name>
```

Runs land in the project folder's `runs/`, which is not in git: a run is rebuilt from its
manifest and seed. The hub shows this scenario at the addresses given above by keeping a
clone of this repository and linking the project folders into its `projects/`.

Free and open source, MIT. The records in `data/events/` keep their publishers' terms,
which each folder's README names.
