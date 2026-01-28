# Copilot Instructions – Homolje (CK3 Mod)

## Überblick & Architektur
- CK3‑Mod mit schlankem Kern: Metadaten in [descriptor.mod](descriptor.mod), Inhalte in `common/` und Lokalisierung in `localization/`.
- Aktuelle Inhalte: Kulturdefinition in [common/culture/cultures/homolje_culture.txt](common/culture/cultures/homolje_culture.txt), Titel in [common/landed_titles/homolje_titles.txt](common/landed_titles/homolje_titles.txt), Texte in [localization/english/homolje_l_english.yml](localization/english/homolje_l_english.yml).

## Wichtige Dateien & Muster
- [descriptor.mod](descriptor.mod): Paradox‑Key/Value‑Format mit Tabs. `supported_version` ist `1.14.*`.
- Kulturkey `homolje` in [common/culture/cultures/homolje_culture.txt](common/culture/cultures/homolje_culture.txt) wird über `culture_homolje*` in [localization/english/homolje_l_english.yml](localization/english/homolje_l_english.yml) lokalisiert.
- Titel `c_homolje` und Baronie `b_kucevo` in [common/landed_titles/homolje_titles.txt](common/landed_titles/homolje_titles.txt) müssen passende `c_homolje*`/`b_kucevo*`‑Einträge in der Lokalisierung haben.

## Projekt‑Konventionen
- Behalte bestehende Einrückung je Datei bei: Tabs in `descriptor.mod` und `*.yml`, Spaces in den `common/`‑Dateien.
- CK3‑Struktur beibehalten (z. B. `common/culture/cultures`, `common/landed_titles`, `localization/english`). Neue Bereiche nur hinzufügen, wenn sie zur Änderung erforderlich sind.

## Workflow
- Keine Build‑/Test‑Skripte. Validierung erfolgt durch Laden im CK3‑Launcher.

## Integrationen
- Keine externen Abhängigkeiten; Integration ausschließlich über die CK3‑Engine/Launcher.
