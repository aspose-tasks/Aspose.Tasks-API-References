---
title: "Enumeratie BookingType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BookingType enumeratie. Specificeert het boekingstype van een resource."
type: docs
weight: 150
url: /nl/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Specificeert het boekingstype van een resource.

```csharp
public enum BookingType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Geeft aan dat de waarde niet gedefinieerd was in het oorspronkelijke projectbestand. |
| Committed | `0` | Geeft het toegezegde boekingstype aan. |
| Proposed | `1` | Geeft het voorgestelde boekingstype aan. |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de eigenschap Asn.BookingType te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


