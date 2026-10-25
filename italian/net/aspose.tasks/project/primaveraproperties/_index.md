---
title: "Project.PrimaveraProperties"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene un oggetto contenente le proprietà specifiche di Primavera per un progetto letto da un file Primavera."
type: docs
weight: 720
url: /it/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Ottiene un oggetto contenente le proprietà specifiche di Primavera per un progetto letto da un file Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Esempi

Mostra come leggere un progetto da un file Primavera ed esaminare le proprietà specifiche di Primavera del progetto.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Restituisce il progetto con UID speciale
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties può essere null se le opzioni di pianificazione del progetto hanno valori predefiniti.
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

### Vedi anche

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


