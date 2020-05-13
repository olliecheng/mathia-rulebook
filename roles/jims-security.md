---
title: Jim's Security
layout: role
alignment: town
enabled: yes
description: Targets 3 players, gets 3 random players and one mafia if one of the targets die
---

Jim's Security, also known as Jim or Camera Man, targets three players each night. If one (or several, see Interactions below) of Jim's targets die during the night, Jim will recieve a list with four alive players: three randomly generated players and one fixed player who was the one that performed the kill. 

There are no restrictions on who the camera man can target.

{% capture interactions %}
Jim's Security > X + Y + Z, Mafia A > X;
Jim gets a list with four players: Random Player 1 + R2 + Mafia A + R3;
The order of the names in the list is random.;

---
Jim's Security > X + Y + Z, Mafia B > X, Thief > Y, Vigilante > Z;
Jim returns "Thief + Mafia B + Random Player 1 + Vigilante";
If two or three of Jim's targets die, then all the players responsible are included in Jim's list.;

---
Jim's Security > X + Y + Z, Mafia A > X, Doctor > X;
Jim's Security returns nothing;
Jim's Security does not get any names since no one was killed.;

{% endcapture %}
{% include interactions.html content=interactions %}
