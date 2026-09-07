---
title: "TaskUtils.Apply"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUtils. Applica l'algoritmo specificato a ciascuna attività di un albero"
type: docs
weight: 10
url: /it/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Applica l'algoritmo specificato a ogni task di un albero.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | Attività | Radice dell'albero |
| alg | ITreeAlgorithm`1 | Algoritmo applicato. |
| livello | Int32 | Livello dell'attività radice. |

## Esempi

Mostra come lavorare con un algoritmo ad albero.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// raccogli tutti i task del progetto
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// lavora con i task come con un semplice elenco
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


