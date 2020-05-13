---
title: Vigilante
layout: role
alignment: town
enabled: yes
description: shoots people
---

Every night the Vigilante has the option of targetting a player of their choice to be killed. However, if the player that they killed is town aligned then they commit suicide the following night.

The Vigilante is not told whether or not the person they targetted was town-aligned.

{% capture interactions %}
Vigilante > Mafia X;
Mafia X dies and the Vigilante does not commit suicide;

---
Vigilante > Executioner;
Executioner dies and the Vigilante does not commit suicide;
The Vigilante does not feel remorse for killing neutral roles so they do not commit suicide;

---
Vigilante > Ordinary Town X;
Ordinary Town X dies and Vigilante commits suicide the next night;

---
Vigilante > Mafia A, Mafia A > Vigilante;
Both the Vigilante and Mafia A die;
The Vigilante shot and the Mafia shot are concurrent;

---
Vigilante > Mafia A, Mafia A > Vigilante, Shaman > Vigilante;
Vigilante dies;
The Vigilante's shot is blocked by the Shaman;

---
Vigilante > Ordinary Town X, Doctor > Ordinary Town X;
Nobody dies and the Vigilante does not commit suicide;
Even though the vigi intended to kill a player who was town-aligned, the Doctor blocked the kill so the Vigilante does not commit suicide;

---
Vigilante > Mafia A, Bus Driver > Mafia A and Ordinary Town X;
Ordinary Town X dies and Vigilante commits suicide the next night;
The Bus Driver causes the Vigilante to shoot Ordinary Town X instead of Mafia, so the Vigilante commits suicide the next night in remorse;
{% endcapture %}
{% include interactions.html content=interactions %}
