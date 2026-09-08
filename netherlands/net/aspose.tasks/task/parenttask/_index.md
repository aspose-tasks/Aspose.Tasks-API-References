---
title: "Task.ParentTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt de bovenliggende taak van een taak op"
type: docs
weight: 940
url: /nl/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Haalt de bovenliggende taak van een taak op.

```csharp
public Task ParentTask { get; }
```

## Voorbeelden

Toont hoe de bovenliggende taak van een taak te gebruiken.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


