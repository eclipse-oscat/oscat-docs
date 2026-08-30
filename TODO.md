# TODO: Vollständige Einsortierung der verbleibenden 98 .md Dateien

## Status

- **98 .md Dateien** aus `en/` sind noch nicht in die Repos einsortiert
- Diese Dateien sind "unmapped" - sie haben keine AixOCAT-Kategorie-Zuordnung
- Sie gehören überwiegend zu **Network** (z.B. base64-*, dlog-*, csv_parser-*) oder **Building** (z.B. air_densitiy, dew_tmp)

## Blocker

Die finale Einsortierung kann erst erfolgen, wenn folgende CODESYS-Produkte verfügbar sind:

1. **CODESYS File Based Storage 1.0.0.0**
   - URL: https://store.codesys.com/de/codesys-file-based-storage.html

2. **CODESYS Git 2.x** (basierend auf File Based Storage)
   - URL: https://store.codesys.com/de/codesys-git.html

## Release-Termin

- **Geplant:** Ende August (lt. CODESYS Release Plan/Roadmap)
- URL: https://www.codesys.com/eco-system/up-to-date/release-lifecycle/release-plan-roadmap/

## Warum warten?

Erst mit File Based Storage und Git 2.x kann sichergestellt werden, dass die Bausteine korrekt ihren jeweiligen OSCAT-Library-Modulen zugeordnet werden. Eine vorzeitige manuelle Zuordnung könnte:

- Zu falschen Kategorien führen
- Nach dem CODESYS-Update neu zugeordnet werden müssen
- Inkonsistenzen zwischen Doku und tatsächlicher Library-Struktur erzeugen

## Betroffene Dateien (Auszug)

```
# Network-Module (vermutlich)
base64.md
base64_decode_str.md
base64_decode_stream.md
base64_encode_str.md
base64_encode_stream.md
csv_parser_buf.md
csv_parser_file.md
dlog.md
dlog_bool.md
dlog_data.md
dlog_dint.md
dlog_dt.md
dlog_file_to_ftp.md
dlog_file_to_smtp.md
dlog_real.md
dlog_store_file_csv.md
dlog_store_file_html.md
...

# Building-Module (vermutlich)
air_densitiy.md
dew_tmp.md
...
```

## Nächste Schritte nach CODESYS-Release

1. File Based Storage installieren
2. Git 2.x installieren
3. OSCAT-Libraries mit neuer Struktur importieren
4. Korrekte Modul-Zuordnung aus CODESYS übernehmen
5. Verbleibende 98 Dateien in `oscat-network-docs` und `oscat-building-docs` einsortieren
6. AixOCAT-mapping.json aktualisieren

---
*Erstellt: Juni 2026*
*Wartet auf: CODESYS File Based Storage 1.0.0.0 + Git 2.x (Release ~Ende August)*
