---
title: "Project.PrimaveraProperties"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene un objeto que contiene propiedades Primaveraspecific para un proyecto leído desde un archivo Primavera"
type: docs
weight: 720
url: /es/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Obtiene un objeto que contiene propiedades específicas de Primavera para un proyecto leído desde un archivo Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Ejemplos

Muestra cómo leer un proyecto desde un archivo Primavera y examinar las propiedades específicas de Primavera del proyecto.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Devuelve el proyecto con UID especial.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties puede ser nulo si las opciones de programación del proyecto tienen valores predeterminados.
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

### Ver también

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


