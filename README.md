# Helia Node

**Deutsch** · [English](#english)

Helia Node ist ein kleiner Dienst für Linux (x64 und arm64). Er macht einen Rechner im eigenen
Betrieb zu einem Helfer für die Helia-App, etwa für lokale Spracherkennung oder lokale KI.

In diesem Repository liegen **nur fertige Programme und ihre Prüfsummen**, kein Quellcode.
Jede Version steht unter [Releases](../../releases) mit vier Dateien:

| Datei | Inhalt |
|---|---|
| `helia-node-linux-x64` | Programm für Intel/AMD (64 Bit) |
| `helia-node-linux-arm64` | Programm für ARM (64 Bit) |
| `install.sh` | Einrichtungs-Skript (systemd) |
| `SHA256SUMS` | Prüfsummen aller Dateien |

## Einrichtung

Die Einrichtung startet man in der **Helia-App** (Einstellungen › Geräte › Server & Nodes ›
Node hinzufügen). Dort steht der passende Befehl mit Kopplungs-Code. Ohne Code aus der App
lässt sich ein Node nicht koppeln.

## Prüfsumme prüfen

```sh
sha256sum -c --ignore-missing SHA256SUMS
```

Jede geladene Datei muss `OK` melden. `install.sh` prüft das Programm vor der Installation
selbst gegen `SHA256SUMS` und bricht bei einer Abweichung ab.

---

## English

Helia Node is a small service for Linux (x64 and arm64). It turns a computer on your own
premises into a helper for the Helia app, for example for local speech recognition or local AI.

This repository contains **only ready-built programs and their checksums**, no source code.
Each version is listed under [Releases](../../releases) with four files:

| File | Contents |
|---|---|
| `helia-node-linux-x64` | Program for Intel/AMD (64-bit) |
| `helia-node-linux-arm64` | Program for ARM (64-bit) |
| `install.sh` | Setup script (systemd) |
| `SHA256SUMS` | Checksums of all files |

### Setup

Setup starts in the **Helia app** (Settings › Devices › Servers & nodes › Add node), which
shows the matching command with a pairing code. A node cannot be paired without a code from
the app.

### Verify the checksum

```sh
sha256sum -c --ignore-missing SHA256SUMS
```

Every downloaded file must report `OK`. `install.sh` also checks the program against
`SHA256SUMS` before installing and stops on any mismatch.
