---
title: "Class RecalculationValidationException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecalculationValidationException class. Vertegenwoordigt een uitzondering die wordt gegooid wanneer fouten in een project worden gevonden na herberekening"
type: docs
weight: 1680
url: /nl/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

Stelt een uitzondering voor die wordt gegooid wanneer er fouten in een project worden gevonden na herberekening.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

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

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


