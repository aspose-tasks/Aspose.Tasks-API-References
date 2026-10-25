---
title: "Tsk.IsSubproject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività è un progetto inserito"
type: docs
weight: 700
url: /it/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Determina se un'attività è un progetto inserito.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


