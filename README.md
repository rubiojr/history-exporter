# Firefox based browsers history exporter

Risor script to export history from Firefox based browsers (Firefox, Waterfox, Pale Moon, etc.) to a CSV file.

## Building

### Pre-requirements

* Go needs to be installed in the system.
* Install RSX from https://github.com/rubiojr/rsx

### Build

Run `rsx build` in the project directory

## Usage

```
Usage: history-exporter <browser-data-dir>
```

Exporting Firefox Linux history:

```
history-exporter ~/.mozilla/firefox > history-firefox.json
```

Exporting LibreWolf flatpak history:

```
history-exporter ~/.var/app/io.gitlab.librewolf-community/.librewolf > history-librewolf.json
```
