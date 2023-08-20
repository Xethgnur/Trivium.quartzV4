---
NoteIcon: District
Settlement: Massarnae
Type: Noble Housing
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
> **Population** | `=this.population` |
> **Theme** | `=this.theme` |
> **Kingdom** | `=link(this.Settlement)` |
> **Terrain** | `=this.terrain` |
> 
> ###### Travel (`=[[Trivium Party Hub]].TravelMethod` for `=[[Trivium Party Hub]].HoursPerDay` hours per day)
> Destination|Travel Days
> ---|---|
> Location|⏱️`= round(1 / (([[Trivium Party Hub]].MilesPerHour * [[Trivium Party Hub]].HoursPerDay) * choice([[Trivium Party Hub]].ExhaustionLevel > 1, 2, 1)) , 2)` days|
> ###### Politics
>  |
> ---|---|
> **Ruler(s)** | `=this.Rulers` |
> **Leaders** | `=this.Leaders` |
> **Defenses** | `=this.defences` |
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

%%
> [!metadata|map]- Map
> ```leaflet
> id: TBD
> image: [[PlaceholderImage.png]]
> height: 600px
> width: 640px
> lat: 50
> long: 50
> minZoom: 1
> maxZoom: 5
> defaultZoom: 1
> unit: meters
> scale: 1
> darkMode: false
> ```
%%

> [!metadata|shops]- Shops
> [[💲 Shop & Service Database|📝Add New Shop/Service]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "Shop")
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
table Pronouns, Party1Standing AS "Motley Few Standing", join(Occupation, ", ") AS "Occupation(s)", join(link(AssociatedGroup), ", ") AS "Group(s)", join(link(AssociatedReligion), ", ") AS "Religion(s)"
WHERE Location = this.file.name AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT file.name ASC


## History


## Notes
### Plot Hooks


### Hidden Details


### General Notes

