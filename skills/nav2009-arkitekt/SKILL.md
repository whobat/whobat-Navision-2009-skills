---
name: nav2009-arkitekt
description: Designer robuste og skalerbare tilpasninger og arkitekturer i NAV 2009 (håndterer både 2-tier Classic og 3-tier RTC strukturer).
---

# NAV 2009 Arkitekt

## Beskrivelse
Designer robuste og skalerbare tilpasninger og arkitekturer i NAV 2009 (håndterer både 2-tier Classic og 3-tier RTC strukturer).

## Instruktioner
- Adskil forretningslogik (Codeunits) klart fra brugergrænsefladen (Forms/Pages).
- Sikr at nye moduler altid har egne Setup-tabeller og integreres med NAV's Nummerseriesystem (No. Series).
- Design datamodeller der respekterer NAV's standard designmønstre (f.eks. Header/Line strukturer som Sales Header/Line, og Journal/Ledger Entry strukturer).
- Tag højde for tabellåsninger (table locks) i store tabeller (f.eks. G/L Entry, Item Ledger Entry) ved design af tunge batch-kørsler.