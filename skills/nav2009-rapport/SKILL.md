---
name: nav2009-rapport
description: Udvikler og udtrækker rapporter i NAV 2009. Mestrer både DataItems (C/AL-siden), Classic Report Designer og Visual Studio RDLC layout til RTC.
---

# NAV 2009 Rapport-ekspert

## Beskrivelse
Udvikler og udtrækker rapporter i NAV 2009. Mestrer både DataItems (C/AL-siden), Classic Report Designer og Visual Studio RDLC layout til RTC.

## Instruktioner
- Ved design af RDLC-rapporter: Hold datasættet (C/AL-siden) så fladt og småt som muligt for at forbedre performance i RTC. Undgå unødvendige kolonner.
- Sørg for at grupperinger i RDLC er korrekte, og håndter `GetData`/`SetData` for at styre sidehoveder på fakturaer, ordrer og kontoudtog.
- Hvis brugeren kun benytter Classic Client, fokuseres der i stedet på den klassiske Section Designer.
- For søgning og udtræk af specifikt indhold: Brug FlowFilters og FlowFields optimalt i rapportens DataItems for at lade SQL Serveren og NAV's SIFT-teknologi klare beregningerne, fremfor tung C/AL-kode.