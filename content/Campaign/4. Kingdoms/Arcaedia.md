---
Pronounced: Arh-kay-dee-ya
Alias: The Land of Forest and Hills, The Arcaedian Dominion
NoteIcon: Kingdom
Theme:
  - Ancient Roman
Terrain:
  - Grassland
  - Forests
  - Mountains
  - Hills
  - Marsh
  - Rivers
Defences: Formidable
GovtType: Federation
Type: Human Kingdom
Continent: Arcaedia
---

> [!infobox]+
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> ![[Arcaedia-1690251900322.jpeg]]
> ###### Info
>  |
> ---|---|
> **Alias** | `=this.alias` |
> **Type** | `=this.type` |
> **Theme** | `=this.theme` |
> **Continent** | `=link(this.Continent)` |
> **Terrain** | `=this.terrain` |
> 
> ###### Travel (`=[[Trivium Party Hub]].TravelMethod` for `=[[Trivium Party Hub]].HoursPerDay` hours per day)
> Destination|Travel Days
> ---|---|
> Wuzhia from Vasaros|⏱️`= round(2390 * ([[Trivium Party Hub]].MilesPerHour * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) / [[Trivium Party Hub]].HoursPerDay / 30, 0)` months|
> Hvergelmir from Vasaros|⏱️`= round(1069 * ([[Trivium Party Hub]].MilesPerHour * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) / [[Trivium Party Hub]].HoursPerDay / 30, 0)` months|
> Amun-Ra from Vasaros|⏱️`= round(2285 * ([[Trivium Party Hub]].MilesPerHour * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) / [[Trivium Party Hub]].HoursPerDay / 30, 0)` months|
> Surinosgar Peaks from Vasaros|⏱️`= round(970 * ([[Trivium Party Hub]].MilesPerHour * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) / [[Trivium Party Hub]].HoursPerDay / 30, 0)` months|
> ###### Politics
>  |
> ---|---|
> **Ruler(s)** | `=this.Rulers` |
> **Leaders** | `=this.Leaders` |
> **Govt Type** | `=this.GovtType` |
> **Defenses** | `=this.defences` |
> **Religion(s)** | `=link(this.religions)` |
> ###### Commerce
>  |
> ---|---|
> **Imports** | `=this.imports` |
> **Exports** | `=this.exports` |
> ###### Groups
>  |
> ---|
[[🔰 Group Database]]
> ```dataview 
table join(Type, ", ") AS Type
WHERE contains(Location, this.file.name) AND contains(NoteIcon, "Group") AND !contains(Type, "Racial Group")
SORT Type ASC

# **`=this.file.name`**
> [!recite]- Introduction
The Arcædian Dominion establishes that it was one of the oldest human territories to have settled themselves and built lasting cities in the Western lands. The Dominion covers almost the entire Western Continent and has enveloped many of the humanoid races together under one banner. The flags of Arcædia are variations of a White Lion roaring, and are colored to each regional major city.


> [!metadata|map]- Map
> ```leaflet
> id: Arcaedia
> image: [[Arcaedia-1690251805794.jpeg]]
> bounds: [[0,0] , [6553.5,4096]]
> height: 1000px
> width: 85%px
> lat: 3276
> long: 2048
> minZoom: -3
> maxZoom: 1
> defaultZoom: -1
> unit: miles
> scale: .3
> ```

> [!metadata|Landmark]- Landmarks
> [[🏰Landmark Database|📝Add New Landmark]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "Landmark")
SORT file.name ASC

> [!metadata|pois]- Points of Interest
> [[❓ POI Database|📝Add New Point of Interest]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "POI")
SORT file.name ASC

> [!metadata|characters]- Characters
> [[👨‍👩‍👧‍👦 NPC Database| 📝Add New NPC]]
> ```dataview
table Pronouns, Party1Standing AS "Party Standing", join(Occupation, ", ") AS "Occupation(s)", join(link(AssociatedGroup), ", ") AS "Group(s)", join(link(AssociatedReligion), ", ") AS "Religion(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT file.name ASC

## Major Cities
- [[Massarnae]]
- [[Phocellis]] 
- [[Varaaros]]
- [[Caronion]]
- [[Thespione]]
- [[Bouroezen]]
- [[Didolllonia]]

## History


## Notes
### Plot Hooks


### Hidden Details


### General Notes

