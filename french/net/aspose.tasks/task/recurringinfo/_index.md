---
title: "Task.RecurringInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient l'instance de la classe RecurringTaskInfo pour la tâche qui est une tâche récurrente ; si la tâche n'est pas récurrente, alors retourne null. Les informations pour l'instance de RecurringTaskInfo sont présentes uniquement au format de fichier mpp."
type: docs
weight: 1030
url: /fr/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

Obtient l'instance de la classe [`RecurringTaskInfo`](../../recurringtaskinfo/) pour la tâche qui est une tâche récurrente ; si la tâche n'est pas récurrente, alors retourne null ; Les informations pour l'instance de [`RecurringTaskInfo`](../../recurringtaskinfo/) sont présentes uniquement au format de fichier mpp.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## Exemples

Montre comment lire les informations récurrentes d'une tâche.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### Voir aussi

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


