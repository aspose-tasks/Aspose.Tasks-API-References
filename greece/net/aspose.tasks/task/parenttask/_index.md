---
title: "Task.ParentTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει την γονική εργασία μιας εργασίας"
type: docs
weight: 940
url: /el/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Λαμβάνει την γονική εργασία μιας εργασίας.

```csharp
public Task ParentTask { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε την γονική εργασία μιας εργασίας.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


