---
title: "Tsk.IsRecurring"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività fa parte di una serie di attività ricorrenti"
type: docs
weight: 670
url: /it/net/aspose.tasks/tsk/isrecurring/
---
## Tsk.IsRecurring field

Determina se un'attività fa parte di una serie di attività ricorrenti.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRecurring;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsRecurring.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRecurring, true);

Console.WriteLine("Is Recurring: " + task.Get(Tsk.IsRecurring));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


