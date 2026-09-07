---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Project-Eigenschaft. Ruft ein Objekt ab, das Primavera-spezifische Eigenschaften für ein aus einer Primavera-Datei gelesenes Projekt enthält."
type: docs
weight: 720
url: /de/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Ruft ein Objekt ab, das Primavera-spezifische Eigenschaften für ein aus einer Primavera-Datei gelesenes Projekt enthält.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Beispiele

Zeigt, wie ein Projekt aus einer Primavera-Datei gelesen und die Primavera-spezifischen Eigenschaften des Projekts untersucht werden können.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Gibt ein Projekt mit spezieller UID zurück.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties kann null sein, wenn die Terminplanungsoptionen des Projekts Standardwerte haben.
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

### Siehe auch

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


