---
NoteIcon: Group
Alignment: Lawful Neutral
HQ:
  - Vasaros
Location:
  - Arcaedia
---

> [!infobox]+
> # `=this.file.name`
> **Pronounced:**  "`=this.Pronounced`"
> ![[Judge of Arcaedia-1691614582411.jpeg]]
> ###### Basic Information
> ###### `=link(this.Hierarchy)`
> Type |  Stat |
> ---|---|
> Alias(es) | `=this.alias` |
> Base of Operations | `=link(this.hq)` |
> Associated Religion | `=link(this.associatedreligion)` |
> Alignment | `=this.alignment` |
> Type | `=this.type` |

# `=this.file.name`
> [!metadata|overview]- Overview
TBD

> [!metadata|settlements]- Locations
> `=link(this.location)`

> [!metadata|landmarks]- Landmarks
> [[Campaign/7. Landmarks/🏰Landmark Database|🏰Add New Landmark]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE contains(AffiliatedGroup, this.file.name) AND contains(NoteIcon, "Landmark")
SORT file.name ASC

> [!metadata|pois]- Points of Interest
> [[❓ POI Database|📝Add New Point of Interest]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE contains(AffiliatedGroup, this.file.name) AND contains(NoteIcon, "POI")
SORT file.name ASC

> [!metadata|shops]- Shops
> [[💲 Shop & Service Database|📝Add New Shop/Service]]
> ```dataview
table join(Type, ", ") AS Type, join(link(AffiliatedGroup), ", ") AS "Group(s)"
WHERE contains(AffiliatedGroup, this.file.name) AND contains(NoteIcon, "Shop")
SORT file.name ASC

> [!metadata|characters]- Characters
> [[👨‍👩‍👧‍👦 NPC Database| 📝Add New NPC]]
> ```dataview
table Pronouns, join(Occupation, ", ") AS "Occupation(s)", join(link(AssociatedGroup), ", ") AS "Group(s)", join(link(AssociatedReligion), ", ") AS "Religion(s)"
WHERE contains(Heritage, this.file.name) OR contains(Ancestry, this.file.name) AND contains(NoteIcon, "Character") AND !contains(Condition, "Dead")
SORT file.name ASC

## Culture
### Mission


### Conduct


### Recruitment & Training


### Ranks


### Uniforms & Equipment


## Acquaintances
### Allies:


### Rivals:


### Contacts:


## History


## Notes
### Plot Hooks


### Hidden Details


### General Notes

