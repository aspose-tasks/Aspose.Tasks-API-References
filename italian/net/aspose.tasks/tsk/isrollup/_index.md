---
title: "Tsk.IsRollup"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se le informazioni sulle barre Gantt della sottoattività saranno aggregate nella barra dell'attività riepilogo"
type: docs
weight: 690
url: /it/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Determina se le informazioni sulle barre Gantt delle sottoattività verranno aggregate nella barra dell'attività riepilogo.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


