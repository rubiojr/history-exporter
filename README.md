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

## Sample output format:

```
❯ ./history-exporter $HOME/.mozilla/firefox/ | jq .[0]
{
  "description": "Guides, information, and news about the Fedora operating system for users, developers, system administrators, and community members.",
  "id": 6,
  "title": "Fedora Magazine - Guides, information, and news about the Fedora operating system for users, developers, system administrators, and community members.",
  "url": "https://fedoramagazine.org/",
  "visit_date": "2024-08-13T16:38:30+02:00",
  "visits": 1
}
```
