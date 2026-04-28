# Agent Skills - Dynamics NAV 2009

Dette repository indeholder en samling af specialiserede agent-skills (færdigheder) til AI-kodningsagenter. Disse skills gør det muligt for agenten at påtage sig forskellige ekspertroller og udføre specifikke opgaver relateret til Microsoft Dynamics NAV 2009 og opgraderinger mod Business Central.

## Inkluderede Skills

- **nav2009-analytiker:** Analyse af forretningsbehov og systemkrav.
- **nav2009-arkitekt:** Systemdesign og løsningsarkitektur.
- **nav2009-bc-ekspert:** Migration og opgradering fra NAV 2009 til Business Central.
- **nav2009-dba:** Databaseadministration og SQL-optimering.
- **nav2009-integrator:** Integrationer og webtjenester.
- **nav2009-koder:** C/AL udvikling og kodning.
- **nav2009-rapport:** Udvikling af rapporter (Classic og RTC/RDLC).
- **nav2009-reviewer:** Code review og kvalitetssikring.

## Installation

Du kan installere disse skills direkte via kommandolinjen, så de bliver tilgængelige for dine AI-agenter.

### Lokal installation (kun for det aktuelle projekt)
For at installere alle NAV 2009 skills lokalt i dit nuværende projekt, kør følgende kommando:
```bash
npx skills add whobat/Navision-2009-skills
```

### Global installation (for alle dine projekter)
For at installere alle NAV 2009 skills globalt, så de er tilgængelige uanset hvilket projekt du arbejder i, kør:
```bash
npx skills add -g whobat/Navision-2009-skills
```

Når installationen er fuldført, vil din agent automatisk kunne benytte disse skills. Du kan for eksempel bede agenten om at *"bruge din nav2009-koder skill til at rette denne fil"*.
