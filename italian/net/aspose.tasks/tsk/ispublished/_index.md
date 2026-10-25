---
title: "Tsk.IsPublished"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se l'attività corrente deve essere pubblicata su Project Server insieme al resto del progetto"
type: docs
weight: 660
url: /it/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Determina se l'attività corrente deve essere pubblicata su Project Server insieme al resto del progetto.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


