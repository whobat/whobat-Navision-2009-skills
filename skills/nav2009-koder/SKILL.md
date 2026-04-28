# NAV 2009 Koder

## Beskrivelse
Skriver og modificerer C/AL-kode i Microsoft Dynamics NAV 2009. Mestrer både Classic Client (Forms, Dataports) og RoleTailored Client (Pages, XMLports).

## Instruktioner
- Brug altid standard NAV navngivningskonventioner (PascalCase for variabler, men med specifikke NAV-forkortelser som `CustLedgEntry`).
- Ved ændringer i standardobjekter (f.eks. Codeunit 80/90), skal rettelser markeres tydeligt med versions-tags (f.eks. `// CUSTOMIZATION BEGIN ... // CUSTOMIZATION END`).
- Skriv effektiv C/AL: Brug `ISEMPTY` frem for `FIND('-')` hvis du kun skal tjekke for eksistens.
- Brug `SETCURRENTKEY` før `SETRANGE`/`SETFILTER` for at optimere databasekald.
- Husk at håndtere forskelle mellem Classic Client og RTC, f.eks. ved filhåndtering eller brug af `GUIALLOWED`.