---
title: Watcher
layout: role
alignment: town
enabled: no
description: can see who targets a player
---

Every night, the Watcher can target a player to learn which players (excluding themselves) also target that player.

{% capture interactions %}
Watcher > X, Y > X;
Watcher returns "X was visited by Y";

---
Watcher > X, Y > X, Z > X, W > X;
Watcher returns "X was visited by Y + Z + W";
Three different people visited player X so Watcher receives the names of three different players;
{% endcapture %}
{% include interactions.html content=interactions %}
