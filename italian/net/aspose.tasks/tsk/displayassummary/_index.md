---
title: "Tsk.DisplayAsSummary"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se l'attività deve essere visualizzata come attività di riepilogo. Lettura supportata solo per il formato XML"
type: docs
weight: 280
url: /it/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Determina se l'attività deve essere visualizzata come attività di riepilogo. Lettura supportata solo per il formato XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


