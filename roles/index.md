---
layout: default
title: Roles Overview
permalink: /roles/
---

Below is a list of the roles, including Power Roles, in Mafia. Some of them may not be in play. While a short summary may be given for each role, click on the link for a more comprehensive description of the role.

<span class="disabled">Gray test like this indicates that the role is not currently in play.</span>


### "Ordinary" Roles
Ordinary roles have no special abilities.

<ul>
{% for page in site.pages %}
{%- assign alignment = page.alignment | downcase -%}
<!-- starts with "ordinary"? -->
{%- assign lowerCaseTitle = page.title | downcase -%}
{% unless lowerCaseTitle == "" %}
{% assign checkArray = lowerCaseTitle | split: "ordinary" %}
{% if checkArray[0] == "" %}
<!-- match! -->
{% assign path = page.path | split: "." | first %}

<li class="{% unless page.enabled %}disabled{% endunless %}">
    <a href="{{ site.baseurl }}../{{ path }}">{{ page.title }}</a>: {{ page.description }}
</li>

{% endif %}
{% endunless %}
{% endfor %}
</ul>



### Town-Aligned Power Roles
These Power Roles have useful abilities which help the Town investigate, prevent, and kill Mafia members.

<ul>
{% for page in site.pages %}
{%- assign alignment = page.alignment | downcase -%}
<!-- starts with "ordinary"? -->
{%- assign lowerCaseTitle = page.title | downcase -%}
{% unless lowerCaseTitle == "" %}
{% assign checkArray = lowerCaseTitle | split: "ordinary" %}
{% unless checkArray[0] == "" %}
<!-- match! -->
{% if alignment == "town" %}
{% assign path = page.path | split: "." | first %}

<li class="{% unless page.enabled %}disabled{% endunless %}">
    <a href="{{ site.baseurl }}../{{ path }}">{{ page.title }}</a>: {{ page.description }}
</li>

{% endif %}
{% endunless %}
{% endunless %}
{% endfor %}
</ul>




### Mafia-Aligned Power Roles
These Power Roles have useful abilities which help the Mafia in disabling the Town's Power Roles.

<ul>
{% for page in site.pages %}
{%- assign alignment = page.alignment | downcase -%}
<!-- starts with "ordinary"? -->
{%- assign lowerCaseTitle = page.title | downcase -%}
{% unless lowerCaseTitle == "" %}
{% assign checkArray = lowerCaseTitle | split: "ordinary" %}
{% unless checkArray[0] == "" %}
<!-- match! -->
{% if alignment == "mafia" %}
{% assign path = page.path | split: "." | first %}

<li class="{% unless page.enabled %}disabled{% endunless %}">
    <a href="{{ site.baseurl }}../{{ path }}">{{ page.title }}</a>: {{ page.description }}
</li>

{% endif %}
{% endunless %}
{% endunless %}
{% endfor %}

</ul>



### Neutral-Aligned Power Roles
These Power Roles all have unique Win Conditions.

<ul>
{% for page in site.pages %}
{%- assign alignment = page.alignment | downcase -%}
<!-- starts with "ordinary"? -->
{%- assign lowerCaseTitle = page.title | downcase -%}
{% unless lowerCaseTitle == "" %}
{% assign checkArray = lowerCaseTitle | split: "ordinary" %}
{% unless checkArray[0] == "" %}
<!-- match! -->
{% if alignment == "neutral" %}
{% assign path = page.path | split: "." | first %}

<li class="{% unless page.enabled %}disabled{% endunless %}">
    <a href="{{ site.baseurl }}../{{ path }}">{{ page.title }}</a>: {{ page.description }}
</li>

{% endif %}
{% endunless %}
{% endunless %}
{% endfor %}

</ul>


The following is a template for making new roles: [New Role Template]({{ site.baseurl }}{% link information/new-role-template.md %})

