# Installation af NAV 2009 Agent Skills

Denne guide beskriver, hvordan du installerer alle NAV 2009 skills korrekt, så din AI-agent (f.eks. `pi`) kan anvende dem. Hver skill består af en undermappe med en `SKILL.md` fil, som indeholder instruktionerne.

## Lokal Installation (Pr. Projekt)

Brug denne metode, hvis du kun vil have adgang til disse skills i et specifikt kodeprojekt. Agenten kigger typisk i `.pi/agent/skills/` i roden af projektet.

1. Opret en mappe til skills i dit nuværende projekt:
   ```bash
   mkdir -p .pi/agent/skills
   ```
2. Kopier mappen med NAV 2009 skills fra dette repository ind i dit projekts skill-mappe:
   ```bash
   cp -r /sti/til/agent-skills-nav2009/skills/* .pi/agent/skills/
   ```

## Global Installation (For Alle Projekter)

Brug denne metode, hvis du vil have at din AI-agent altid skal have adgang til disse skills, uanset hvilket projekt du arbejder i. For `pi` ligger globale skills typisk i din brugerprofils `.pi`-mappe.

### Windows
1. Åbn PowerShell og opret skill-mappen:
   ```powershell
   New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.pi\agent\skills\"
   ```
2. Kopier alle skills ind i den globale mappe:
   ```powershell
   Copy-Item -Path "C:\sti\til\agent-skills-nav2009\skills\*" -Destination "$env:USERPROFILE\.pi\agent\skills\" -Recurse
   ```

### macOS / Linux
1. Opret den globale skill-mappe:
   ```bash
   mkdir -p ~/.pi/agent/skills/
   ```
2. Kopier skills over:
   ```bash
   cp -r /sti/til/agent-skills-nav2009/skills/* ~/.pi/agent/skills/
   ```

## Anvendelse

Når de er installeret, vil agenten automatisk indlæse dem som tilgængelige færdigheder. Du kan aktivere dem ved at referere til dem i din prompt, f.eks.:
- *"Brug din `nav2009-koder` skill til at rette denne Codeunit."*
- *"Du skal agere som `nav2009-arkitekt` og komme med et forslag til integrationen."*
