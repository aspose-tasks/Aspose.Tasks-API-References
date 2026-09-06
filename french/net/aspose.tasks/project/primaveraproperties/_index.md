---
title: "Project.PrimaveraProperties"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient un objet contenant les propriétés spécifiques à Primavera pour un projet lu à partir d'un fichier Primavera"
type: docs
weight: 720
url: /fr/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Obtient un objet contenant les propriétés spécifiques à Primavera pour un projet lu à partir d'un fichier Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Exemples

Montre comment lire un projet à partir d'un fichier Primavera et examiner les propriétés spécifiques à Primavera du projet.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Renvoie le projet avec un UID spécial
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties peut être nul si les options d'échéancier du projet ont des valeurs par défaut.
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

### Voir aussi

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


