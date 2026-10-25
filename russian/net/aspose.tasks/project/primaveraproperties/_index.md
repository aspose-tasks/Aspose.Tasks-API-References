---
title: "Project.PrimaveraProperties"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает объект, содержащий специфические для Primavera свойства проекта, считанные из файла Primavera."
type: docs
weight: 720
url: /ru/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Получает объект, содержащий свойства, специфичные для Primavera, для проекта, считанного из файла Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## Примеры

Показывает, как прочитать проект из файла Primavera и изучить специфические для Primavera свойства проекта.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Возвращает проект со специальным UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// PrimaveraProperties может быть null, если параметры расписания проекта имеют значения по умолчанию.
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

### См. также

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


