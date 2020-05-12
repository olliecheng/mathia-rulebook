---
title: Executioner
layout: role
alignment: neutral
enabled: yes
description: must get their assigned target lynched to win, has no abilities
---

At the start of the game, a random player is chosen as the Executioner's _target_. The Executioner's win condition is to successfully lynch their target. When this happens, the identity of the Executioner is revealed. It is then publicly announced that they have won, and they are removed from the game.

If the target dies in any way other than being lynched, the Executioner (if alive) becomes a Jester. 

{% capture interactions %}
Detective > Executioner;
Detective returns "Innocent";
Neutral roles show up as innocent to the detective;
{% endcapture %}
{% include interactions.html content=interactions %}
