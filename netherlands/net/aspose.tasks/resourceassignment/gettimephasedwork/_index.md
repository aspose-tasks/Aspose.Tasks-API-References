---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment-methode. Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval"
type: docs
weight: 730
url: /nl/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Begin van het datum‑tijdinterval. |
| einde | DateTime | Einde van het datum‑tijdinterval. |
| timephasedDataType | TimephasedDataType | Type van de tijdgephaseerde gegevens die gebruikt moeten worden. |

## Voorbeelden

Toont hoe je het werk van een toewijzing berekent voor een willekeurig datum‑tijdinterval.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Print het werk van de toewijzing voor elk uur.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Zie ook

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Begin van het datum‑tijdinterval. |
| einde | DateTime | Einde van het datum‑tijdinterval. |

### Zie ook

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


