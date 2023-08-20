---
Pronounced: Mah-sar-nay
Alias: The Lumbering Castle o' the Woods
NoteIcon: Settlement
Type: Large City
Population: "16184"
Theme:
  - Medieval
Kingdom: Arcaedia
Terrain:
  - Forest
  - Hills
Defences: Average
GovtType: Oligarchy
Imports:
  - Grain
Exports:
  - Lumber
---

> [!infobox]+
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> ![[Massarnae-1690253860495.jpeg]]
> ###### Info
>  |
> ---|---|
> **Alias** | `=this.alias` |
> **Type** | `=this.type` |
> **Population** | `=this.population` |
> **Theme** | `=this.theme` |
> **Kingdom** | `=link(this.Kingdom)` |
> **Terrain** | `=this.terrain` |
> 
> ###### Travel (`=[[Trivium Party Hub]].TravelMethod` for `=[[Trivium Party Hub]].HoursPerDay` hours per day)
> Destination|Travel Days
> ---|---|
> [[Dragon's Head]] |⏱️`= round(90 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
> [[Vasaros]] |⏱️`= round(600 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
> [[Phocellis]] |⏱️`= round(440 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
> [[Bouroezen]] |⏱️`= round(720 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
> [[Thimbleville]] |⏱️`= round(1225 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
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
WHERE econtains(Location, this.file.name) AND contains(NoteIcon, "Group")
SORT Type ASC

# **`=this.file.name`**
> [!recite]- Introduction
TBD

> [!metadata|map]- Map
> ```leaflet
> id: Massarnae
> image: ![[Massarnae-1690253889412.jpeg]]
> bounds: [[0,0],[1365.19,1230.38]]
> height: 600px
> width: 640px
> lat: 683
> long: 615
> minZoom: -1
> maxZoom: 1
> defaultZoom: 0
> unit: meters
> scale: 1.1
> darkMode: false
> ```

> [!metadata|districts]- Districts
> [[🌁 Districts Database| 📝Add New District]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AssociatedReligion), ", ") AS "Religion(s)"
WHERE Settlement = this.file.name AND contains(NoteIcon, "District")
SORT file.name ASC

> [!metadata|shops]- Shops
> [[💲 Shop & Service Database|📝Add New Shop/Service]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "Shop")
SORT file.name ASC

> [!metadata|pois]- Points of Interest
> [[❓ POI Database|📝Add New Point of Interest]]
> ```dataview
table join(Type, ", ") AS Type, join(link(Owner), ", ") AS "Owner(s)"
WHERE Settlement = this.file.name AND contains(NoteIcon, "POI")
SORT file.name ASC

> [!metadata|characters]+ Characters
> [[👨‍👩‍👧‍👦 NPC Database| 📝Add New NPC]]
>> [!cards|dataview 5]
>>```dataview
TABLE WITHOUT ID
>>	embed(Art) AS "Art",
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>	condition AS "Condition"
WHERE contains(NoteIcon, "Character") AND contains(Type, "NPC") AND !contains(Condition, "Dead") AND contains(Location, this.file.name)
>>SORT file.name asc
>>```

## History


## Notes
### Plot Hooks


### Hidden Details


### General Notes

