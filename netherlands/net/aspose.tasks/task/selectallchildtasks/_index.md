---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakmethode. Verzamelt recursief alle onderliggende taken van deze taak."
type: docs
weight: 1400
url: /nl/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Verzamelt recursief alle onderliggende taken van deze taak.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Retourwaarde

Een lijst met onderliggende taken van deze taak.

## Voorbeelden

Toont hoe over onderliggende taken geïtereerd kan worden.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


