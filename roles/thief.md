---
title: Thief
layout: role
alignment: neutral
enabled: yes
description: steals abilities to win
---

The thief wins by stealing three unique items from different targets. Each night, the thief may choose someone not chosen previously to steal from and see if they receive an item. The thief can steal the following items:

- **Mafia Gun** from an Ordinary Mafia
- **Staff** from Shaman
- **Vigilante's Gun** from Vigilante
- **CAT scanner** from Doctor
- **Magnifying Glass** from Detective
- **Voodoo Doll** from Voodoo Doll

Additionally, if the Thief has successfully stolen an item the previous night, they may choose to use the item during the next night action concurrent with mafia shot. 

**A player that is stolen from, is unable to use their stolen item the following night. The thief's steal goes AFTER all other night actions.**

If more than one ordinary mafia member is alive and one of them gets stole from one night, the other mafia member can still kill during the next night. Different mafia guns are indistinguishable and stealing several mafia guns does not increase the number of uniquely stolen items for the thief. In gang war mafia there is no difference between the guns of the different mafias or the staffs of the different shamans. Since killings in the game is concurrent a thief stealing their third item while being killed the same night still wins.

{% capture interactions %}

Thief > Mafia A, Mafia A > Thief;
Thief dies and does not get gun;
Thief's steal goes after mafia shot;

---
Thief > Mafia A (shoots), Mafia A > Thief;
Both mafia and thief die;
Thief's item use is concurrent with mafia shot;

---
Thief > X (saves), Thief > Shaman (steal), Mafia A > X;
X does not die, Thief receives staff from shaman;
Thief's item use is concurrent with mafia shot;

---
Thief > Detective, Detective > Thief;
Thief gets a magnifying glass and detective returns "Innocent";
Neutral roles show up as innocent to the detective;

---
Thief > Town X (investigate), Thief > Mafia A (steal), Shaman > Thief;
Thief gets that Town X is guilty and does not get anything from Mafia A;
Shaman reverses detective's result even when the magnifying glass is stolen. Shaman also roleblocks the thief from stealing so they don't get anything from the mafia.;

{% endcapture %}
{% include interactions.html content=interactions %}
