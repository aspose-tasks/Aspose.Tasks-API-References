---
title: "Tsk.IsActive"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività è attiva. Le attività inattive non influenzano più le altre attività né la pianificazione complessiva del progetto"
type: docs
weight: 550
url: /it/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Determina se un'attività è attiva. Le attività inattive non influenzano più altre attività né la programmazione complessiva del progetto.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


