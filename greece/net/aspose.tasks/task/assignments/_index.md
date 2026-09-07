---
title: "Task.Assignments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει μια συλλογή από αναθέσεις πόρων για αυτό το αντικείμενο"
type: docs
weight: 120
url: /el/net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Λαμβάνει μια συλλογή από αναθέσεις πόρων για αυτό το αντικείμενο.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις αναθέσεις της εργασίας.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // εμφάνιση των αναθέσεων της εργασίας
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Δείτε επίσης

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


