---
title: Thief
layout: role
alignment: neutral
enabled: yes
description: steals abilities to win
---

The thief wins by stealing sufficient items from different targets. Each night, the thief may choose someone not chosen previously to steal from and see if they receive an item. All roles with night actions have an item (e.g. mafia, doctor) while power roles without night actions do not (executioner, mason). Items stolen from power roles with distinct night actions will be distint (e.g. mafia gun and vigilante gun are indistinguishable while doctor's item is distinguishable). Additionally, if the thief has successfully stolen an item the previous night, he may choose to use the item during the next night action concurrent with mafia shot. The thief's steal goes AFTER all other night actions.  

{% capture interactions %}
Thief > mafia A, mafia A > Thief;
Thief dies and does not get gun;
Thief's steal goes after mafia shot;

---
Thief > mafia A (shoots), mafia A > thief;
Both mafia and thief die;
Thief's item use is concurrent with mafia shot;

---
Thief > X (saves), Thief > Shaman (steal), Mafia A > X;
X does not die, Thief receives staff from shaman;
Thief's item use is concurrent with mafia shot;

{% endcapture %}

Check out [Contributing]({{ site.baseurl }}{% link information/contributing.md %}) to see how to fill in this role!
