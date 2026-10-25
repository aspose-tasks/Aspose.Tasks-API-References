---
title: "Tsk.IsNull"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività è un'attività nulla"
type: docs
weight: 640
url: /it/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Determina se un'attività è un'attività nulla.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


