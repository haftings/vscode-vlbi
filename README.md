# VLBI File Types

This VSCode extension provides file type support for several Very Long Baseline Interferometry (VLBI) file types.

## File Types (Languages) Supported

* Haystack Observatory Postprocessing System (HOPS) Configuration File (CF)
* VLBI Correlator Report
* VLBI Master Schedule file
* VLBI Stations files (`ns-codes.txt`, `m.stations`, and `stations.m`)

## Installation

Just copy these files into `~/.vscode/extensions` and restart Code.

```bash
rsync -vac --delete /path/to/vlbi-file-types/ ~/.vscode/extensions/vlbi-file-types/
```

## Known Issues

* VLBI Correlator Report
  * The first column of a table header may be syntax highlighted as a key name
    (e.g. from a dictionary section) if it starts with a capital leter
  * The `FRINGING_CONFIG_FILE` section will always try to syntax highlight
    as a HOPS CF file, even if it is a different fringing config format

## Planned Features

* Additional language support
  * NASA SKED session schedule file
  * VLBI Experiment (VEX) session schedule file
  * DiFX VEX to DiFX (V2D) configuration file
  * DiFX `input` and related files
