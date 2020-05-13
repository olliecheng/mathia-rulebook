---
title: Suicide Bomber
layout: role
alignment: town
enabled: yes
description: Undefendably kills people while killing themselves
---

Every night the Suicide Bomber has the opportunity to kill a player of their choice while commiting suicide themselves. This action occurs before any of the other night actions, making it completely undefendable.

{% capture interactions %}
Suicide Bomber > Mafia X;
Mafia X and the Suicide Bomber die;

---
Suicide Bomber > Town X, Doctor > Town X, Shaman > Suicide Bomber, Bus Driver > Mafia Y and Town X;
Town X and the Suicide Bomber die;
The Doctor, the Shaman and the Bus Driver are all unable to prevent the Suicide Bomber's kill since their night actions occur afterwards;
{% endcapture %}
{% include interactions.html content=interactions %}
