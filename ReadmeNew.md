# Kryoschlaf‑Simulation — Öffentliche Zusammenfassung

## Kurzbeschreibung
Aggregierte Ergebnisse einer erweiterten Monte‑Carlo‑Simulation zur Robustheit von Kryokapseln (500 Runs, 5 Jahre). Vollständiger Code und Rohdaten sind privat; dieses Repo veröffentlicht nur die wichtigsten Kennzahlen, Annahmen und Empfehlungen.

## Kernergebnisse
| Metrik | Wert |
|---|---:|
| Total Runs | 500 |
| Zeithorizont | 5 Jahre (1825 Tage) |
| Überlebensrate | ≈ 99.7 % |
| Mean End‑Muscle | ≈ 19.2 % |
| Std End‑Muscle | ≈ 1.4 |
| Median End‑Muscle | ≈ 19.1 % |
| 5. Perzentil | ≈ 17.2 % |
| 95. Perzentil | ≈ 21.1 % |

## Modell‑Kurzbeschreibung
- Power Policy: Batterie + Aggregat schützen 7 Tage + 3 Tage Puffer; ein Backup ausgefallen → Wake‑Up nach 4 Tagen; beide ausgefallen → sofortiges Notaufwecken.  
- Notaufwach‑KI: priorisiert Wake‑Up nach medizinischer Dringlichkeit.  
- Synthetisches Blut: modellierte Reduktion der Thrombose‑Wahrscheinlichkeit und leichte O₂‑Effizienzsteigerung.  
- Redundanz: dreifache Pumpen, doppelte Ventile, Wartungszyklen, Cyber‑ und Human‑Error‑Ereignisse.

## Top‑Sensitivitätsfaktoren
1. Thrombose‑Wahrscheinlichkeit  
2. Common‑Cause Failure Rate (CCF)  
3. Pumpen‑Ausfallrate  
4. KI‑Rescue‑Erfolg  
5. Wake‑Capacity

## Limitierungen & Validierung
- Klinische Validierung des synthetischen Bluts erforderlich.  
- Feldmessungen für MTBF und KI‑Erfolg empfohlen.  
- Modellannahmen sind stochastisch und abstrahieren reale Komplexität.

## Kontakt
Bei berechtigtem Interesse an Code oder Rohdaten bitte per E‑Mail an: [kontakt@example.org]
