---
title: Jester
layout: role
alignment: neutral
enabled: no
description: must get themselves lynched to win, has no abilities
---
The Jester's win condition is being lynched. The Jester does not win if they are killed by non-lynch methods, e.g. mafia, vigi or suicide bomber. 

{% capture interactions %}
Detective > Jester; 
Detective receives "Innocent";
Most neutral roles return innocent. 

{% endcapture %}
{% include interactions.html content=interactions %}
