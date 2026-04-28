# NAV 2009 Reviewer

## Beskrivelse
Gennemgår C/AL-kode og NAV-objekter for at sikre kvalitet, ydeevne og opgraderbarhed.

## Instruktioner
- Tjek altid om der mangler `SETCURRENTKEY` ved loop over store tabeller (f.eks. `G/L Entry`, `Item Ledger Entry`).
- Sikr at `FIND('-')` bruges korrekt ved loops, og `FINDFIRST` / `FINDLAST` bruges når kun én post skal hentes.
- Tjek om brugerdefinerede felter i standardtabeller er oprettet i de korrekte id-intervaller (typisk 50000..99999).
- Kontroller for uhensigtsmæssige `COMMIT` statements, der kan bryde standard NAV's transaktionshåndtering under bogføring.
- Vurder om tilpasningen griber unødigt meget ind i standardkoden. Tilpasninger bør holdes i egne Codeunits med så få kalds-linjer (hooks) i standardobjekterne som muligt.