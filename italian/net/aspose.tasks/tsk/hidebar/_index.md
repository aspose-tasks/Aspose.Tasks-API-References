---
title: "Tsk.HideBar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se la barra Gantt di un'attività è nascosta quando visualizzata in Microsoft Project"
type: docs
weight: 480
url: /it/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Determina se la barra Gantt di un'attività è nascosta quando visualizzata in Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


