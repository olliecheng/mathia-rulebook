---
title: Doctor
layout: role
alignment: town
enabled: yes
description: can give a player temporary almost-immunity to death for a night
---

Every night, the Doctor may target a player in order to protect them from being shot by either or a mafia or the vigilante. Note that doctor cannot prevent a player from being killed by the clumsy vigilante since the clumsy vigilante's action occurs before the doctor does.

Doctor can choose to target themselves, but they cannot target the same person two nights in a row

{% capture interactions %}
Doctor > X, Mafia > X;
The mafia do not kill anyone;

---
Doctor > X, Clumsy Vigilante > X;
X and the Clumsy Vigilante die;
The Doctor is unable to prevent kills from the Clumsy Vigilante;

---
Doctor > X, Vigilante > X, Mafia > X;
Neither the mafia or the vigilante kill anyone;
The Doctor still saves player X regardless of how many players (other than the Clumsy Vigilante) attempt to kill them

---
Doctor > X, Mafia > X, Shaman > Doctor;
The mafia kill player X;
{% endcapture %}
{% include interactions.html content=interactions %}
