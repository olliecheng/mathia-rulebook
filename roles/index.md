---
layout: default
title: Roles Overview
permalink: /roles/
---

Below is a list of the roles, including Power Roles, in Mafia. Some of them may not be in play. While a short summary may be given for each role, click on the link for a more comprehensive description of the role.

## Understanding the "Interactions" Section
An example Interaction will look like this:

> - **`Detective → X`, `Shaman → Detective`** _(L1)_  
> **Result: `Detective returns "Shaman'd"`** _(L2)_  
> If Shaman targets Detective, the Detective's action is blocked, and they are made aware of this. _(L3)_

L1 are the "input parameters" i.e. what happens. The format is this: `Player A → Player B` means that Player A targets Player B with their action. The assumption is that Player A is not roleblocked and not reversed i.e. the action actually happens. If a player is given as `X`, `Y`, `A`, `B`, or other, it represents any player who will be represented using that letter.

L2 is the result. `Player A returns "string"` means that Player A is privately told, "string". If other players have been mentioned as a target or another power role in L1, but they are not explicitly listed in L2, they are not told anything.

L3 is an explanation for why this interaction exists.

### "Ordinary" Roles
Ordinary roles have no special abilities.
- [Ordinary Town]({% link roles/ordinary-town.md %})
- [Ordinary Mafia]({% link roles/ordinary-mafia.md %})
- _there is no Neutral aligned ordinary role._

### Town-Aligned Power Roles
These Power Roles have useful abilities which help the Town investigate, prevent, and kill Mafia members.
- [Detective]({% link roles/detective.md %}): investigates a player every night to determine alignment
- [Doctor]({% link roles/doctor.md %}): can give a player temporary immunity for a night
- [Vigilante and Suicide Bomber]({% link roles/vigilante-and-suicide-bomber.md %}): shoots people
- [Tracker]({% link roles/tracker.md %}): can see who a player targets
- [Watcher]({% link roles/watcher.md %}): can see who targets a player

### Mafia-Aligned Power Roles
These Power Roles have useful abilities which help the Mafia in disabling the Town's Power Roles.
- [Shaman]({% link roles/shaman.md %}): also called a **roleblocker**, the Shaman can disable a player's abilities for a night
- [Bus Driver]({% link roles/bus-driver.md %}): pulls the ol' switcheroo and swaps around players so that PRs target the wrong person
- [Traitor]({% link roles/traitor.md %}): has no ability, a nerfed Mafia player without a vote in mafia kills and doesn't know who the Mafia are

### Neutral-Aligned Power Roles
These Power Roles all have unique Win Conditions.
- [Thief]({% link roles/thief.md %}): steals abilities to win
- [Jester]({% link roles/jester.md %}): must get themselves lynched to win, has no abilities
- [Executioner]({% link roles/executioner.md %}): must get their assigned target lynched to win, has no abilities

The following is a template for making new roles: [New Role Template]({% link information/new-role-template.md %})

