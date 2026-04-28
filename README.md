# Agent Skills - Dynamics NAV 2009

Dette repository indeholder en samling af specialiserede "Agent Skills" til AI-kodningsagenter (som Pi, Claude Code, GitHub Copilot m.fl., der understøtter Agent Skills standarden). Disse skills gør det muligt for agenten at påtage sig forskellige ekspertroller og udføre specifikke opgaver relateret til Microsoft Dynamics NAV 2009 og opgraderinger mod Business Central.

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

Dette repository overholder den officielle **[Agent Skills Specification](https://agentskills.io/specification)**, hvilket betyder, at du kan installere skills automatisk via det universelle `skills` CLI-værktøj eller manuelt til din agent.

### Metode 1: Brug af "skills" CLI (Anbefalet til Claude, Copilot osv.)
Sørg for at du har [Node.js](https://nodejs.org/) installeret. Hvis du oplever fejl med `npx` (f.eks. `cb.apply is not a function`), anbefales det at installere `skills` globalt først:

```bash
# 1. Installer skills CLI (hvis du ikke allerede har det)
npm install -g skills

# 2. Installer NAV 2009 skills lokalt (kun i dit nuværende projekt):
skills add whobat/whobat-Navision-2009-skills

# ...eller globalt (for alle dine projekter):
skills add -g whobat/whobat-Navision-2009-skills
```

### Metode 2: Direkte i Pi (eller andre agenter via Git)
Hvis du bruger en agent som **Pi**, kan du klone repositoriet direkte ind i agentens skill-mappe:

**Globalt (virker i alle projekter):**
```bash
git clone https://github.com/whobat/whobat-Navision-2009-skills.git ~/.pi/agent/skills/whobat-nav2009-skills
```

**Lokalt (kun nuværende projekt):**
```bash
mkdir -p .pi/skills
git clone https://github.com/whobat/whobat-Navision-2009-skills.git .pi/skills/whobat-nav2009-skills
```

Når installationen er fuldført, vil din agent automatisk kunne opdage og benytte disse skills i sit system-prompt.
