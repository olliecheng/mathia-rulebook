---
title: Shaman
layout: role
alignment: mafia
enabled: yes
description: can disable a player’s abilities for a night
---

Every night, the Shaman may choose a player to prevent them from performing any action that night.

Additionally, if the Shaman targets the same person that the detective targets then the detective will receive the reversed result to usual.

Shaman and Ordinary Mafia do not share a private channel, but they both know each other's identities.

{% capture interactions %}
Shaman > Doctor, Doctor > Player X, Mafia > Player X;
Player X dies;
Doctor was blocked from saving Player X by the Shaman;

---
Shaman > Mafia X, Detective > Mafia X;
Detective returns "X is innocent";
Shaman and Detective target the same person so the true investigation result is reversed;

---
Shaman > Town X, Detective > Town X;
Detective returns "X is guilty";
Shaman and Detective target the same person so the true investigation result is reversed;

{% endcapture %}
{% include interactions.html content=interactions %}
