---
title: Detective
layout: role
---

> **🏡 Town Aligned**

Every night, the Detective can choose a target to investigate. They will be informed whether the target is guilty.

### Interactions
- `Detective → Town Aligned`,  
 **Result:** `Detective returns "Not Guilty"`
- `Detective → Mafia Aligned`  
 **Result:** `Detective returns "Guilty"`
- `Detective → Neutral Aligned`  
 **Result:** `Detective returns "Not Guilty"`
- `Detective → X`, `Shaman → Detective`  
 **Result:** `Detective returns "Shaman'd"`  
 If Shaman targets Detective, the Detective's action is blocked, and they are made aware of this.  
- `Detective → X`, `Shaman(s) → X`  
**Result:** `Detective returns the opposite result to normally`  
Unless targetted by another shaman, in which case Detective returns "Shaman'd"