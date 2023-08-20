---
NoteIcon: POI
Type: House
Terrain:
  - Urban
Owner: "[[Tyrian Cromwell]]"
Settlement: Dragon's Head
---

> [!infobox]+
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> ![[PlaceholderImage.png]]
> ###### Info
>  |
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
> [[Mysterious Cave]] |⏱️`= round((210/1609) / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 3) * 1440` minutes
> ###### Ownership
>  |
> ---|---|
> **Religion(s)** | `=link(this.religions)` |
> **Owner**| [[Tyrian Cromwell]]
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

