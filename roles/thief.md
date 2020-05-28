---
title: Thief
layout: role
alignment: neutral
enabled: yes
description: steals abilities to win
---

The thief wins by stealing three unique items from different targets. Each night, the thief may choose someone not chosen previously to steal from and see if they receive an item. The thief can steal the following items:

- **Revolver** from an Ordinary Mafia
- **Staff** from Shaman
- **Sniper Rifle** from Vigilante
- **CAT Scanner** from Doctor
- **Magnifying Glass** from Detective
- **Bomb** from Big Bomb Bob (Bomber)

Additionally, if the Thief has successfully stolen an item the previous night, they may choose to use the item during the next night action concurrent with mafia shot. 

**A player that is stolen from, is unable to use their stolen item the following night. The thief's steal goes AFTER all other night actions.**

If more than one ordinary Mafia member is alive and one of them gets stolen from one night, the other Mafia member can still kill during the next night. Different Mafia revolvers are indistinguishable and stealing several mafia revolvers does not increase the number of uniquely stolen items for the thief. In Gang War Mafia (i.e. multiple Mafia factions) there is no difference between the revolvers of the different Mafias, or the staffs of the different shamans.

{% capture interactions %}

Thief > Mafia A, Mafia A > Thief;
Thief dies and does not get revolver;
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
Thief gets that "No result" and does not get anything from Mafia A;
Shaman blocks Detective investigation. Shaman also roleblocks the Thief from stealing, so they don't get anything from the mafia.;

{% endcapture %}
{% include interactions.html content=interactions %}
