---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Προωθεί μια εργασία στο περίγραμμα"
type: docs
weight: 1390
url: /el/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Προωθεί μια εργασία στο περίγραμμα.

```csharp
public void OutlineOutdent()
```

## Παραδείγματα

Δείχνει πώς να αφαιρέσετε εσοχή από μια εργασία.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// αφαιρέστε εσοχή από την εργασία
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


