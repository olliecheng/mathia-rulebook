---
title: Jim's security
layout: role
alignment: town
enabled: yes
description: Targets 3 players, gets 3 random players and one mafia if one of the targets die
---

Jim's security, also known as jim or camera man, targets three players each night. If one (or several, see interactions below) of Jim's targets die during the night, Jim will recieve a list with four alive players: three randomly generated players and one fixed player who was the one that performed the kill. 

The last games Tracker have recieved nothing when they investigate Jim's security. This could, however, change (that tracker for example recieves one of jim's targets, randomly generated) so make sure to check with GMs (game masters) if you are unsure :)

There are no restrictions on who the camera man can target.

{% capture interactions %}
Jim's security > X + Y + Z, Mafia A > X;
Jim gets a list with four players: p1 + p2 + Mafia A + p3;
The order of the names in the list is random

---
Jim's security > X + Y + Z, Mafia B > X, Thief > Y, Vigilante > Z;
Jim gets a list with four players: Thief + Mafia B + p1 + Vigilante;
If two or three of the Jim's targets die two or three of the names in the list are the players who performed the kill.;

---
Jim's Security > X + Y + Z, Mafia A > X, Doctor > X;
Jim's security does not get any names;
Jim's security does not get any names since no one was killed. If Mafia A had been a suicide bomber Jim would get results since the suicide bomber performs their kill before other PR (power role) actions.

{% endcapture %}
{% include interactions.html content=interactions %}
