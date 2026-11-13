# Arbeitsanweisungen für Age of Mythology: Retold

## Einstieg und Arbeitsweise

- Unteragenten sind für Chats in diesem Projekt ausdrücklich erlaubt und sollen
  nach eigenem Ermessen eingesetzt werden, wenn dies für die Aufgabe sinnvoll ist.
- Zuerst [Documentation/README.md](Documentation/README.md) lesen. Für Datenmods
  zusätzlich [Gameplay Data](Documentation/Gameplay_Data.md), für XS, Karten, KI
  oder Trigger [XS and Scenarios](Documentation/XS_and_Scenarios.md), für Modelle,
  UI oder Audio [Assets and Editor](Documentation/Assets_and_Editor.md) lesen.
- Die installierte Steam-Version, den Snapshot und vorhandene Änderungen prüfen,
  bevor Spielfelder, IDs, Skriptsignaturen oder Modverhalten vorausgesetzt werden.
  Die Pfade und den Aktualisierungsablauf enthält [Local Snapshot](Documentation/Local_Snapshot.md).
- Unterstützte Daten-, Skript-, Editor- und Asset-Schnittstellen zuerst untersuchen.
  Für eine konkrete offene Frage zuerst offizielle Handbücher und Patchnotes,
  aktuelle Daten oder Skripte sowie vorhandene Mods heranziehen. Community-Berichte
  und ältere Builds mit Herkunft und Gültigkeitsbereich einordnen. Native Analyse
  nur als gesonderte Untersuchung einer Frage, die damit offen bleibt.
- Datendateien nur additiv ändern, wenn das jeweilige Format und der betroffene
  Knoten es unterstützen. Interne Namen für neue Inhalte eindeutig wählen und
  unnötige Überschneidungen mit anderen Mods vermeiden. Feste IDs aus älteren
  Konstantenlisten vor der Verwendung gegen den aktuellen Kontext prüfen.
- Modarbeit findet in ihrem eigenen Modordner statt. Bestehende lokale Änderungen,
  andere Mods und die Steam-Installation bei Analyse und Tests erhalten. Die
  Spieldatenextrakte und mitgelieferten Handbücher bleiben lokale Referenzen.

## Prüfen und dokumentieren

- Nach Datenänderungen XML und Referenzen statisch prüfen. Für einen Spieltest
  zunächst im lokalen Profil isoliert testen, relevante Logs und bei additiven
  Änderungen die zusammengeführten Daten prüfen. Mehrspieler, Editor, DLC und
  gespeicherte Partien gezielt prüfen, wenn die Änderung sie betrifft.
- In der englischen Dokumentation gesicherte Erkenntnisse mit Build, genauer
  Quelle und Prüfstatus ergänzen. Statische Prüfung, dokumentierte Absicht,
  historischer Versuch und beobachtetes Spielverhalten getrennt ausweisen.
- Beim Refresh nur die betroffenen Quellen neu erfassen und den geprüften
  Extrakt mit dem neuen Stand ersetzen. Bei Fehlern den vorherigen Stand
  behalten und die Abweichung dokumentieren. Commits und Veröffentlichung nur
  auf ausdrücklichen Auftrag.
