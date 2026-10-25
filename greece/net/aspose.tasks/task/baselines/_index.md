---
title: "Task.Baselines"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ή ορίζει τη συλλογή των τιμών βάσης της εργασίας"
type: docs
weight: 130
url: /el/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Λαμβάνει ή ορίζει τη συλλογή των τιμών baseline της εργασίας.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις βάσεις της εργασίας.

```csharp
var project = new Project();

// ορίστε μια βάση
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Εμφάνιση διάρκειας βάσης αναφοράς εργασίας
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Δείτε επίσης

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


