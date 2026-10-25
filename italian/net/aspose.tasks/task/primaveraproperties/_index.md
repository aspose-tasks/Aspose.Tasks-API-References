---
title: "Task.PrimaveraProperties"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene un oggetto contenente le proprietà specifiche di Primavera per un task letto da un file Primavera"
type: docs
weight: 1010
url: /it/net/aspose.tasks/task/primaveraproperties/
---
## Task.PrimaveraProperties property

Ottiene un oggetto contenente proprietà specifiche di Primavera per un'attività letta dal file Primavera.

```csharp
public PrimaveraTaskProperties PrimaveraProperties { get; }
```

## Esempi

Mostra come leggere un progetto da un XML di Primavera ed esaminare le proprietà specifiche di Primavera dei task.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3883;

// Restituisce il progetto con UID speciale
var project = new Project(DataDir + "PrimaveraProject.xml", options);

foreach (Task task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("Task '{0}'", task.Name);

    if (task.IsSummary)
    {
        Console.WriteLine("WBS Sequence number: {0}", task.PrimaveraProperties.SequenceNumber);
    }
    else
    {
        Console.WriteLine("Task ActivityId: {0}", task.PrimaveraProperties.ActivityId);
    }

    Console.WriteLine("Activity Type: {0}", task.PrimaveraProperties.ActivityType);
    Console.WriteLine("Duration Type: {0}", task.PrimaveraProperties.DurationType);
    Console.WriteLine("Percent Complete Type: {0}", task.PrimaveraProperties.PercentCompleteType);
    Console.WriteLine("Original Duration: {0:N2}", task.Duration.TimeSpan.TotalHours);
    Console.WriteLine("At Complete Duration: {0:N2}", task.ActualDuration.TimeSpan.TotalHours + task.RemainingDuration.TimeSpan.TotalHours);
    Console.WriteLine("Duration % Complete: {0}", task.PrimaveraProperties.DurationPercentComplete);
    Console.WriteLine("Physical % Complete: {0}", task.PrimaveraProperties.PhysicalPercentComplete);

    Console.WriteLine("Task RemainingEarlyStart: {0}", task.PrimaveraProperties.RemainingEarlyStart);
    Console.WriteLine("Task RemainingEarlyFinish: {0}", task.PrimaveraProperties.RemainingEarlyFinish);

    Console.WriteLine("Labor Units:");
    Console.WriteLine("{0}, {1}, {2}, {3}", 
        task.PrimaveraProperties.ActualLaborUnits,
        task.PrimaveraProperties.ActualNonLaborUnits,
        task.PrimaveraProperties.RemainingLaborUnits,
        task.PrimaveraProperties.RemainingNonLaborUnits);

    Console.WriteLine("Actual costs:");
    Console.WriteLine("{0}, {1}, {2}, {3}, Total: {4}",
        task.PrimaveraProperties.ActualExpenseCost,
        task.PrimaveraProperties.ActualLaborCost,
        task.PrimaveraProperties.ActualMaterialCost,
        task.PrimaveraProperties.ActualNonlaborCost,
        task.PrimaveraProperties.ActualTotalCost);

    Console.WriteLine("Constraints:");
    Console.WriteLine("Primary: {0}, {1}", task.PrimaveraProperties.PrimaryConstraintType, task.PrimaveraProperties.PrimaryConstraintDate);
    Console.WriteLine("Secondary: {0}, {1}", task.PrimaveraProperties.SecondaryConstraintType, task.PrimaveraProperties.SecondaryConstraintDate);

    Console.WriteLine("Units % Complete: {0}", task.PrimaveraProperties.UnitsPercentComplete);
}
```

### Vedi anche

* class [PrimaveraTaskProperties](../../primaverataskproperties/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


