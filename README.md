# Agent Skills - Dynamics NAV 2009

Dette repository indeholder en samling af specialiserede "Agent Skills" til AI-kodningsagenter som **GitHub Copilot**, **Claude Code**, **Cursor**, **Windsurf**, **Pi** og mange andre. Disse skills gør det muligt for din AI-agent at påtage sig forskellige ekspertroller og udføre specifikke opgaver relateret til Microsoft Dynamics NAV 2009 og opgraderinger mod Business Central.

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

Dette repository overholder den officielle **[Agent Skills Specification](https://agentskills.io/specification)**. Du kan derfor nemt installere det via det universelle `skills` CLI-værktøj, som automatisk sørger for at integrere dem i din foretrukne AI-assistent.

### Metode 1: Automatisk installation med "skills" CLI (Anbefalet)
Det officielle `skills` CLI-værktøj kan automatisk installere disse skills i GitHub Copilot, Claude Code, Cursor m.fl.

Sørg for at du har [Node.js](https://nodejs.org/) installeret og kør derefter:

```bash
# 1. Installer CLI-værktøjet (undgår npx-fejl på ældre systemer):
npm install -g skills

# 2. For at installere i dit nuværende projekt:
skills add whobat/whobat-Navision-2009-skills

# ...eller for at installere globalt (tilgængeligt i alle projekter):
skills add -g whobat/whobat-Navision-2009-skills
```
*Tip: CLI-værktøjet opdager selv hvilke agenter (f.eks. Copilot eller Claude) du bruger, og sætter filerne op det rigtige sted.*

### Metode 2: Manuel installation via Git
Hvis du foretrækker ikke at bruge et CLI-værktøj, kan du klone repositoriet ind i den standardiserede mappe for agent skills:

**Lokalt (kun i dit nuværende projekt):**
```bash
mkdir -p .agents/skills
git clone https://github.com/whobat/whobat-Navision-2009-skills.git .agents/skills/whobat-nav2009-skills
```

**Globalt (virker for alle dine projekter):**
```bash
# Opret den globale mappe (Linux/Mac bruger ~/.agents, Windows bruger %USERPROFILE%\.agents)
mkdir -p ~/.agents/skills
git clone https://github.com/whobat/whobat-Navision-2009-skills.git ~/.agents/skills/whobat-nav2009-skills
```

Når installationen er fuldført, vil din valgte AI-agent automatisk læse filerne og have adgang til den indbyggede NAV 2009-viden i sine instruktioner.
