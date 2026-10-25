---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De agenda van een resource"
type: docs
weight: 190
url: /nl/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

De agenda van een resource.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Voorbeelden

Toont hoe een resourceagenda opgehaald/ingesteld kan worden.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Voeg een standaardagenda toe en wijs toe aan een resource
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Toon basiskalendernaam voor alle resources
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


