---
title: "Task.OutlineIndent"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Indenta un'attività nella struttura"
type: docs
weight: 1380
url: /it/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Indenta un'attività nella struttura.

```csharp
public void OutlineIndent()
```

## Esempi

Mostra come indentare un'attività.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// indenta l'attività
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


