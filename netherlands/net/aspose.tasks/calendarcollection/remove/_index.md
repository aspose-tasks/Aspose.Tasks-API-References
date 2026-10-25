---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection-methode. Verwijdert een agenda uit Project CalendarCollection"
type: docs
weight: 60
url: /nl/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Verwijdert Calendar uit de Project CalendarCollection.

```csharp
public bool Remove(Calendar item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | Calendar | De agenda die verwijderd moet worden. |

### Retourwaarde

Als verwijderd, retourneert true, anders false.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| InvalidOperationException | Wordt gegooid wanneer de agenda niet kan worden verwijderd. |

## Voorbeelden

Toont hoe je een agenda in de collectie vervangt.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// voeg nieuwe agenda toe
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


