---
title: Coroner
layout: role
alignment: town
enabled: yes
description: Can see the role of dead people
---

Every night the Coroner may choose a player who has already died. They receive the role of the targetted dead player.
{% capture interactions %}
Coroner > Mafia X (dead);
Coroner returns "X was Mafia";

---
Coroner > Doctor X (dead);
Coroner returns "X was Doctor";

---
Coroner > Detective (dead), Shaman > Coroner;
Coroner returns "No result";
{% endcapture %}
{% include interactions.html content=interactions %}
