---
title: Big Bomb Bob
layout: role
alignment: town
enabled: yes
description: (also called the Bomber) undefendably kills people while killing themselves
---

Every night the Big Bomb Bob (also known as the Bomber) has the opportunity to kill a player of their choice while commiting suicide themselves. This action occurs before any of the other night actions, making it completely undefendable.

{% capture interactions %}
Bomber > Mafia X;
Mafia X and the Bomber die;

---
Bomber > Town X, Doctor > Town X, Shaman > Bomber, Bus Driver > Mafia Y and Town X;
Town X and the Bomber die;
The Doctor, the Shaman and the Bus Driver are all unable to prevent the Bomber's kill since their night actions occur afterwards;
{% endcapture %}
{% include interactions.html content=interactions %}
