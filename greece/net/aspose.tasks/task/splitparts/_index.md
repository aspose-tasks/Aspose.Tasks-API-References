---
title: "Task.SplitParts"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει μια συλλογή SplitPart που αντιπροσωπεύει τα τμήματα μιας εργασίας"
type: docs
weight: 1110
url: /el/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Λαμβάνει μια συλλογή SplitPart που αντιπροσωπεύει τα τμήματα μιας εργασίας.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Παραδείγματα

Δείχνει πώς να εμφανίσετε τα τμήματα μιας εργασίας.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Πρόσβαση στην εργασία 
var task = project.RootTask.Children.GetById(4);

// Εμφάνιση τμημάτων της εργασίας
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Δείτε επίσης

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


