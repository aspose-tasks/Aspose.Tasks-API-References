---
title: "Tsk.LevelAssignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se la funzione di livellamento può ritardare e suddividere le assegnazioni individuali per risolvere le sovrallocazioni"
type: docs
weight: 750
url: /it/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Determina se la funzione di livellamento può ritardare e suddividere le assegnazioni individuali per risolvere le sovrassegnazioni.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


