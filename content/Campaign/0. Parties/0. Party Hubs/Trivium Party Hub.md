---
alias: the party, The party
TravelMethod: On Foot
HoursPerDay: 8
ExhaustionLevel: 0
MilesPerHour: 2.5
---

# **Trivium of Time**
> [!metadata|party] Party
 🧙‍♂️[[🧙‍♂️ Party Database| Edit Party]] | 👨‍👩‍👧‍👦[[👨‍👩‍👧‍👦 NPC Database | Edit NPCs]]
>> [!cards|dataview 5] **Party**
>>```dataview
TABLE WITHOUT ID
>>	embed(Art) AS "Art",
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>	pronouns AS "Pronouns",
>>	ancestry AS "Ancestry",
>>	heritage AS "Heritage",
>>	condition AS "Condition",
>>	link(location, location) AS "Location"
WHERE contains(NoteIcon, "Character") AND contains(WhichParty, "Party 1") AND !contains(Condition, "Dead")
>>SORT file.name asc
>>```

> [!metadata|sessionlogs]+ Session Logs
📝[[📝 Session Note Database| New Session Log]]
>> [!cards|dataview 3]
>>```dataview
TABLE WITHOUT ID
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Date + "</span>" AS Date,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Alias + "</span>" AS Alias,
>>	QuickNotes AS "QuickNotes"
WHERE contains(NoteIcon, "SessionNote") AND contains(WhichParty, "Party 1")
>>SORT file.name desc LIMIT 3
>>```

> [!metadata|holdings]+ Ownership
❓[[❓ POI Database | New Point Of Interest]] | 🏰[[Campaign/7. Landmarks/🏰Landmark Database| New Landmark]] | 💲[[💲 Shop & Service Database| New Shop/ Service]]
>> [!cards|dataview 3]
>>```dataview
>> TABLE WITHOUT ID
>>	embed(Art) AS "Art",
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; text-align: center; margin-bottom: 5px;'>" + link(file.link, Location) + "</span>" AS Location
>> WHERE contains(NoteIcon, "Landmark") OR contains(NoteIcon, "Shop") OR contains(NoteIcon, "POI")AND contains(WhichParty, "Party1")
>>SORT file.name desc
>>```

> [!metadata|quests]+ Quests
❗[[❗ Quest Database | New Main Quest]]
>> [!cards|dataview 3]
>>```dataview
TABLE WITHOUT ID
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Status + "</span>" AS Status,
>>	QuickNotes AS "QuickNotes"
WHERE contains(NoteIcon, "Quest") AND contains(WhichParty, "Party1") AND contains(status, "Active")
>>SORT file.name asc
>>```

> [!metadata|sidequests]+ Side Quests
❓[[❗ Quest Database | New Side Quest]]
>> [!cards|dataview 3]
>>```dataview
TABLE WITHOUT ID
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Status + "</span>" AS Status,
>>	QuickNotes AS "QuickNotes"
WHERE contains(NoteIcon, "Side") AND contains(WhichParty, "Party1") AND contains(status, "Active")
>>SORT file.name asc
>>```

> [!metadata|servicerequests]+ Service Requests
🏷️[[🎫 Service Request Database | New Service Request]]
>> [!cards|dataview 3]
>>```dataview
TABLE WITHOUT ID
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Status + "</span>" AS Status,
>>	QuickNotes AS "QuickNotes"
WHERE contains(NoteIcon, "ServiceRequest") AND contains(WhichParty, "Party1") AND contains(status, "Requested") OR contains(status, "In-Progress") OR contains(status, "Pending Pick-Up")
>>SORT file.name asc
>>```

> [!metadata|letters]+ Letters
✉️[[✉️ Letter Database| New Letter]]
>> [!cards|dataview 3]
>>```dataview
TABLE WITHOUT ID
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + link(file.link, Title) + "</span>" AS Title,
>>     "<span style='display: block; border-bottom: 2px solid var(--accent); text-align: center; margin-bottom: 5px;'>" + Status + "</span>" AS Status,
>>	QuickNotes AS "QuickNotes"
WHERE contains(NoteIcon, "Letter") AND contains(WhichParty, "Party1") AND !contains(status, "Complete")
>>SORT file.name asc
>>```

## **Notes**
