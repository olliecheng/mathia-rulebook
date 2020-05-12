---
title: Bus Driver
layout: role
alignment: mafia
enabled: no
description: pulls the ol’ switcheroo and swaps around players so that PRs target the wrong person
---

Every night, the Bus Driver may target two players. If any player then targets one of those two players they will actually end up targetting the other one of those two players.

A player that targets a player that gets targeted by the bus driver is not informed that their targeted player was also targeted by the bus driver.

{% capture interactions %}
Bus Driver > Mafia X + Town Y, Detective > Mafia X;
Detective returns "innocent";
Unbeknownst to the detective, they actually targeted Player Y, so they got the result "innocent" when in fact the player they intended to target was guilty

---
Bus Driver > C + D, Jim's Security > A + B + C;
Jim's security ends up targeting A, B, and D;

---
Watcher > A, Bus Driver > A;
Watcher returns "Nobody visited";
The Bus Driver is effectively invisible to the Watcher.
{% endcapture %}
{% include interactions.html content=interactions %}
