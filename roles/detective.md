---
title: Detective
layout: role
alignment: town
enabled: yes
description: investigates a player every night to determine alignment
---
 
Every night, the Detective can target a player to learn about whether that player is "innocent" or "guilty". In general, mafia-aligned players are counted as guilty but neutral and town-aligned players are counted as innocent. See the individual role descriptions to confirm whether or not that role returns a guilty result when targetted by detective.

Detective has a special interaction with shaman. If the shaman and the detective target the same person then the detective receives the opposite result to what they usually would have.

{% capture interactions %}
Detective > Ordinary Town X,;
Detective returns "X is innocent";

---
Detective > Executioner X,;
Detective returns "X is innocent";

---
Detective > Mafia X,;
Detective returns "X is guilty";

---
Detective > Traitor X,;
Detective returns "X is innocent";
Traitor is considered innocent for balancing purposes;

---
Detective > Mafia X, Shaman > Detective;
Detective does not receive a result;
Detective was role-blocked by shaman;

---
Detective > Town X, Shaman > Town X;
Detective returns "X is guilty";
Shaman and Detective target the same person so the true investigation result is reversed
{% endcapture %}
{% include interactions.html content=interactions %}
