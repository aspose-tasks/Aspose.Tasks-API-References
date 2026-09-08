---
title: "Klasse TaskValidationException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskValidationException klasse. Vertegenwoordigt een uitzondering die wordt gegooid wanneer fouten worden gevonden in projecttaken na herberekening"
type: docs
weight: 2510
url: /nl/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Stelt een exceptie voor die wordt gegooid wanneer fouten worden gevonden in de taken van een project na herberekening.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Haalt de taak op die de uitzondering veroorzaakte. |

## Voorbeelden

Toont onder welke voorwaarden de &lt;see cref="TaskValidationException" /&gt; uitzondering kan worden gegooid.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // per ongeluk onjuiste datums instellen
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // voer projectherberekening uit met een vlag om validatie uit te voeren   
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Zie ook

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


