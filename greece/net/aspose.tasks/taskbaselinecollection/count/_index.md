---
title: "TaskBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TaskBaselineCollection. Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο TaskBaselineCollection"
type: docs
weight: 10
url: /el/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο TaskBaselineCollection.

```csharp
public int Count { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές baseline εργασιών.

```csharp
var project = new Project();

// δημιουργήστε baseline έργου
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// εκτυπώστε baseline εργασιών
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// ας καθαρίσουμε όλα τα baseline
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Δείτε επίσης

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


