# VLBI File Types

This VSCode extension provides file type support for several Very Long Baseline Interferometry (VLBI) file types.

## File Types (Languages) Supported

* Haystack Observatory Postprocessing System (HOPS) Configuration File (CF)
* VLBI Master Schedule file
* VLBI Stations files (`ns-codes.txt`, `m.stations`, and `stations.m`)

## Installation

Just copy these files into `~/.vscode/extensions` and restart Code.

```bash
rsync -vac --delete /path/to/vlbi-file-types/ ~/.vscode/extensions/vlbi-file-types/
```
