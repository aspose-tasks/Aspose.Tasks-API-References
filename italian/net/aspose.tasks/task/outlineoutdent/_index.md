---
title: "Task.OutlineOutdent"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Promuove un'attività nella struttura"
type: docs
weight: 1390
url: /it/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Promuove un'attività nella struttura.

```csharp
public void OutlineOutdent()
```

## Esempi

Mostra come ridurre il rientro di un'attività.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// riduci il rientro dell'attività
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


