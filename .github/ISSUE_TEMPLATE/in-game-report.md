---
name: In-Game Report
about: Report an incident that happened in Minecraft.
title: ''
labels: ''
assignees: ''

---

name: Player Report
description: Report an In-Game rule-breaker
title: "[Player Report]: "
labels: ["in-game"]
body:
  - type: markdown
    attributes:
      value: |
        Please select the clause of our rules violated on the right-hand side if you can classify it. (Optional) 
  - type: input
    id: name
    attributes:
      label: Player Name
      description: Please specify the In-Game name of the player you would like to report
      placeholder: ex. patbeni
  - type: dropdown
    id: reason
    attributes:
      label: Could you describe the type or rule-breaking in one word?
      options:
        - Cheating
        - Abuse
        - Trolling
        - Chat Offenses
  - type: textarea
    id: 
    attributes:
      label: Describe what happened
      description: Describe what happened when you had your encounter with the rule breaker, if possible, mention what kind of client modifications they used (if they did).
      placeholder: Tell us what you see!
    validations:
      required: true
  - type: dropdown
    id: minigame
    attributes:
      label: Minigame
      description: What Minigame did you play when you encountered the rule-breaker?
      options:
        - SkyWars Solo
        - SkyWars Duo
        - BedWars Solos
        - Bedwars Duos
        - BedWars Trios
        - BedWars Squads
        - TheLab
        - Village Defense   
    validations:
      required: true
  - type: dropdown
    id: reason
    attributes:
      label: Could you describe the type or rule-breaking in one word?
      options:
        - Cheating
        - Abuse
        - Trolling
        - Chat Offenses
  - type: checkboxes
    id: personal
    attributes:
      label: For Personal Issues
      description: In case your issue is highly personal, you can choose to not press charges, therefore we will not issue a punishment.
      options:
        - label: Do not press charges
          required: false
