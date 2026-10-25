---
title: "Tsk.SubprojectName"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La posizione di origine di un sotto-progetto"
type: docs
weight: 1070
url: /it/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

La posizione di origine di un sotto-progetto.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Esempi

Mostra come creare un'attività di sotto-progetto.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Aggiungi attività
var task = project.RootTask.Children.Add("Task 1");

// Impostazione nuovo collegamento al sotto-progetto
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


