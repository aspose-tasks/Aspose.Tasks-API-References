---
title: "TaskUtils.TaskChildrenCount"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUtils. Calcola ricorsivamente il numero di attività figlie attraverso tutti i livelli"
type: docs
weight: 40
url: /it/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Calcola ricorsivamente il numero di task figli di un task attraverso tutti i livelli.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attività | Attività | L'attività di cui si calcolano i figli. |

### Valore di ritorno

Il numero di figli.

## Esempi

Mostra come usare il metodo &lt;see cref=\"Aspose.Tasks.Util.TaskUtils.TaskChildrenCount\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// calcola ricorsivamente il numero di attività figlie di un'attività attraverso tutti i livelli
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


