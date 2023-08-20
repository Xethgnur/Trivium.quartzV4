---
NoteIcon: POI
Terrain:
  - Cavernous
  - Forest
Type: Cave
Settlement: Dragon's Head
---

> [!infobox]+
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> 
> ###### Info
>  |![[mysteriousCavern.png]]
> ---|---|
> **Alias** | `=this.alias` |
> **Type** | `=this.type` |
> **Theme** | `=this.theme` |
> **Location** | [[Dragon's Head]] |
> **Terrain** | `=this.terrain` |
> 
> ###### Travel (`=[[Trivium Party Hub]].TravelMethod` for `=[[Trivium Party Hub]].HoursPerDay` hours per day)
> Destination|Travel Days
> ---|---|
> [[Dragon's Head]] |⏱️`= round((200/1609) / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 3) * 1440` minutes
> ###### Politics
>  |
> ---|---|
> **Religion(s)** | `=link(this.religions)` |
> ###### Commerce
>  |
> ---|---|
> **Exports** | `=this.exports` |
> ###### Groups
>  |
> ---|
[[🔰 Group Database]]
> ```dataview 
table join(Type, ", ") AS Type
WHERE econtains(Location, this.file.name) AND contains(NoteIcon, "Group")
SORT Type ASC

# **`=this.file.name`**
> [!recite]- Introduction
TBD

## History


## Notes
### Plot Hooks


### Hidden Details


### General Notes

