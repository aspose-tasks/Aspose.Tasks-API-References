---
title: "Tsk.PhysicalPercentComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Valore di percentuale completata che può essere usato come alternativa per calcolare il costo preventivato del lavoro eseguito (BCWP)"
type: docs
weight: 900
url: /it/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Valore di percentuale completata che può essere usato come alternativa per calcolare il costo preventivato del lavoro eseguito (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


