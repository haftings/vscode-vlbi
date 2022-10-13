# VLBI File Types

This VSCode extension provides file type support for several Very Long Baseline Interferometry (VLBI) file types.

## File Types (Languages) Supported
* DiFX `input`, `calc`, and `im` configuration files
* DiFX VEX to DiFX (V2D) configuration file
* Haystack Observatory Postprocessing System (HOPS) Configuration File (CF)
* NASA SKED session schedule file
* VLBI Correlator Report
* VLBI Master Schedule file
* VLBI Stations files (`ns-codes.txt`, `m.stations`, and `stations.m`)

## Installation and Maintinence

Just copy these files into `~/.vscode/extensions` and restart Code.

* Install:

  ```bash
  git clone https://github.com/haftings/vscode-vlbi ~/.vscode/extensions/vlbi
  ```

* Update:

  ```bash
  (cd ~/.vscode/extensions/vlbi && git fetch && git pull)
  ```

* Uninstall:

  ```bash
  rm -rf ~/.vscode/extensions/vlbi
  ```

## Known Issues

* VLBI Correlator Report
  * The first column of a table header may be syntax highlighted as a key name
    (e.g. from a dictionary section) if it starts with a capital leter
  * The `FRINGING_CONFIG_FILE` section will always try to syntax highlight
    as a HOPS CF file, even if it is a different fringing config format
  * The `CORRELATION_CONFIG_FILE` section will always try to syntax highlight
    as a DiFX V2D file, even if it is a different correlation config format
* NASA SKED session schedule file
  * Keywords are far from exhaustive, and there are probably many missing


## Planned Features

* Additional language support
  * VLBI Experiment (VEX) session schedule file
