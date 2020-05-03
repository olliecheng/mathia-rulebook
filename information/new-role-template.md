---
title: New Role Template
layout: role
alignment: neutral
enabled: yes
permalink: /new-role-template/
---

<br>
<br>

{% raw %}
```
---
title: <name of role>
layout: role
alignment: town OR mafia OR neutral
enabled: yes OR no
---

<Description of the role goes here.>

{% capture interactions %}

Mafia A > Vigilante, Vigilante > Mafia A;  <-- SEMICOLON, COMMA SEPARATED
X dies, Vigilante dies;                    <-- SEMICOLON, COMMA SEPARATED
Explanation goes here;                     <-- SEMICOLON
                       <-- this blank line is optional :)
---                    <-- THREE LINES FOR A NEW INTERACTION
Tracker > Mafia A, Mafia B kill > X;       <-- SEMICOLON, COMMA SEPARATED
Tracker returns "Did not visit anybody";   <-- SEMICOLON, QUOTES
The Tracker did not track the Mafia member who performed the kill (that was Mafia B);  <-- SEMICOLON

{% endcapture %}
{% include interactions.html content=interactions %}
```
{% endraw %}


<Description of the role goes here.>

{% capture interactions %}

Mafia A > Vigilante, Vigilante > Mafia A;
X dies, Vigilante dies;
Explanation goes here;

--- 
Tracker > Mafia A, Mafia B kill > X;
Tracker returns "Did not visit anybody";
The Tracker did not track the Mafia member who performed the kill (that was Mafia B);

{% endcapture %}
{% include interactions.html content=interactions %}