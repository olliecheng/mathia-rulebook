---
title: Ordinary Mafia
layout: role
alignment: mafia
enabled: yes
description: the informed minority
special: ordinary
---

The Ordinary Mafia members have a private channel in which they can talk to each other. Every night, they nominate a member among themselves to kill a specific player of their choosing. It is only this nominated member that can be seen to target someone by tracker/watcher or show up in jim's security's list.


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

---
Mafia A > X, Jim's Security > X + Y + Z, Watcher > X, Tracker > Mafia B;
X dies, Jim's Security returns a list with "A + B + C + Mafia A", Watcher returns "Mafia A visited X", Tracker returns "Did not visit anybody"
{% endcapture %}
{% include interactions.html content=interactions %}
