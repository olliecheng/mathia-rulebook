---
title: Ordinary Mafia
layout: role
alignment: mafia
enabled: yes
description: the informed minority
special: ordinary
---

The Ordinary Mafia have a private channel in which they can talk to each other. Every night, they nominate a member among themselves to kill a specific player of their choosing.

{% capture interactions %}
Ordinary Mafia A > X;
X dies;

---
Detective > Ordinary Mafia A;
Detective returns "Guilty";

---
Ordinary Mafia A > X, Doctor > X;
No one dies;
The player who the mafia attempted to kill was saved by the Doctor;
{% endcapture %}
{% include interactions.html content=interactions %}
