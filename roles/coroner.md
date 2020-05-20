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

---
Coroner > Italian Mafia X (dead);
Coroner returns "X was Italian Mafia";
Coroner is made aware of the faction of the Mafia if there are multiple factions.;

{% endcapture %}
{% include interactions.html content=interactions %}
