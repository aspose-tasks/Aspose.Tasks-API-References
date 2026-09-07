---
title: "Class RecalculationValidationException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.RecalculationValidationException class. Rappresenta un'eccezione che viene lanciata quando vengono trovati errori nel progetto dopo la ricalcolazione"
type: docs
weight: 1680
url: /it/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

Rappresenta un'eccezione che viene lanciata quando vengono trovati errori nel progetto dopo il ricalcolo.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

## Esempi

Mostra in quali condizioni l'eccezione &lt;see cref=\"TaskValidationException\" /&gt; può essere lanciata.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // impostare accidentalmente date errate
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // eseguire la ricalcolazione del progetto con un flag per eseguire la convalida
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Vedi anche

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


