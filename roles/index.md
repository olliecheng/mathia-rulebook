---
layout: default
title: Roles Overview
permalink: /roles/
---

Below is a list of the roles, including Power Roles, in Mafia. Some of them may not be in play. While a short summary may be given for each role, click on the link for a more comprehensive description of the role.

<span class="disabled">Gray text like this indicates that the role is not currently in play.</span>


### "Ordinary" Roles
Ordinary roles have no special abilities.

<ul>
{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=ordinary"
                                     param3="enabled=yes"
                                     template='<li><a href="$url">$title</a>: $description</li>' %}

{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=ordinary"
                                     param3="enabled=no"
                                     template='<li class="disabled"><a href="$url">$title</a>: $description</li>' %}
</ul>



### Town-Aligned Power Roles
These Power Roles have useful abilities which help the Town investigate, prevent, and kill Mafia members.

<ul>
{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=yes"
                                     param4="alignment=town"
                                     template='<li><a href="$url">$title</a>: $description</li>' %}

{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=no"
                                     param4="alignment=town"
                                     template='<li class="disabled"><a href="$url">$title</a>: $description</li>' %}
</ul>





### Mafia-Aligned Power Roles
These Power Roles have useful abilities which help the Mafia in disabling the Town's Power Roles.

<ul>
{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=yes"
                                     param4="alignment=mafia"
                                     template='<li><a href="$url">$title</a>: $description</li>' %}

{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=no"
                                     param4="alignment=mafia"
                                     template='<li class="disabled"><a href="$url">$title</a>: $description</li>' %}
</ul>



### Neutral-Aligned Power Roles
These Power Roles all have unique Win Conditions.

<ul>
{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=yes"
                                     param4="alignment=neutral"
                                     template='<li><a href="$url">$title</a>: $description</li>' %}

{% include function.fetch-pages.html param1="layout=role"
                                     param2="special=empty"
                                     param3="enabled=no"
                                     param4="alignment=neutral"
                                     template='<li class="disabled"><a href="$url">$title</a>: $description</li>' %}
</ul>

<br>

The following is a template for making new roles: [New Role Template]({{ site.baseurl }}{% link information/new-role-template.md %})

