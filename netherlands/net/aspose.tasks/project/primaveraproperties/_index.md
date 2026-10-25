---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt een object op dat Primavera‑specifieke eigenschappen bevat voor een project dat is gelezen uit een Primavera‑bestand"
type: docs
weight: 720
url: /nl/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Haalt een object op dat Primavera-specifieke eigenschappen bevat voor een project dat uit een Primavera-bestand is gelezen.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Voorbeelden

Toont hoe een project uit een Primavera‑bestand te lezen en de Primavera‑specifieke eigenschappen van het project te onderzoeken.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Retourneert project met speciale UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties kan null zijn als de planningsopties van het project standaardwaarden hebben.
if (project.PrimaveraProperties != null)
{
    Console.WriteLine("Project's schedule options:");
    Console.WriteLine("Relationship Lag Calendar: " + project.PrimaveraProperties.RelationshipLagCalendar);
    Console.WriteLine("Make Open Ended Activities Critical: " + project.PrimaveraProperties.MakeOpenEndedActivitiesCritical);
    Console.WriteLine("Ignore Other Project Relationships: " + project.PrimaveraProperties.IgnoreOtherProjectRelationships);
    Console.WriteLine("Use Expected Finish Dates: " + project.PrimaveraProperties.UseExpectedFinishDates);

    Console.WriteLine("How critical activities are defined: " +
                      project.PrimaveraProperties.CriticalActivitiesDefiningMethod);

    if (project.PrimaveraProperties.CriticalActivitiesDefiningMethod == PrimaveraCriticalActivitiesDefiningMethod.TotalFloat)
    {
        Console.WriteLine("Total Float threshold for critical activities: " + project.PrimaveraProperties.CriticalTotalFloatLimit);
    }
}
```

### Zie ook

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


