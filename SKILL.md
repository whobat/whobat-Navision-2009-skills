---
name: nav2009-skills
description: Overordnet installations- og overbliksværktøj for alle Microsoft Dynamics NAV 2009 under-skills.
---

# Navision 2009 Skills - Paraply Skill

## Description
Denne skill fungerer som et overordnet installations- og overbliksværktøj for alle Microsoft Dynamics NAV 2009 under-skills (`nav2009-analytiker`, `nav2009-arkitekt`, `nav2009-bc-ekspert`, `nav2009-dba`, `nav2009-integrator`, `nav2009-koder`, `nav2009-rapport`, `nav2009-reviewer`). 

Den gør det muligt for agenter at installere alle under-skills på én gang.

## Agent Instructions

Når brugeren beder dig (agenten) om at installere "Navision 2009 skills" direkte via en prompt (hvis de ikke allerede har brugt CLI-værktøjet), skal du udføre følgende trin for at sikre at alle de relevante undermapper bliver tilgængelige som individuelle skills.

1. **Find kildemappen:**
   Find `skills/` biblioteket i dette repository (samme mappe hvor denne `SKILL.md` befinder sig, blot i undermappen `skills`).

2. **Bestem destination:**
   - **Lokalt (standard):** Brug `.pi/agent/skills/` i brugerens arbejdsbibliotek. Opret mappen, hvis den ikke findes (`mkdir -p .pi/agent/skills/`).
   - **Globalt:** Hvis brugeren eksplicit beder om en global installation via dig, brug `~/.pi/agent/skills/` (Linux/macOS) eller `$env:USERPROFILE\.pi\agent\skills\` (Windows).

3. **Udfør kopieringen:**
   Kopier alle mapper i kildemappen (`skills/*`) til destinationen. Eksempel på kommando:
   ```bash
   cp -r <sti-til-dette-repo>/skills/* <destinationsmappe>/
   ```

4. **Bekræft over for brugeren:**
   Når kopieringen er afsluttet, skal du informere brugeren om, at alle NAV 2009-rollerne (som analytiker, koder, dba osv.) nu er installeret og klar til brug, og at de kan tilgås som individuelle skills.
