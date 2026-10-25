---
title: "ChildTasksCollector.Alg"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ChildTasksCollector. Elabora l'oggetto specificato"
type: docs
weight: 30
url: /it/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Elabora l'oggetto specificato.

```csharp
public override void Alg(Task el, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | Attività | Oggetto da elaborare. |
| livello | Int32 | Livello del nodo dell'albero. |

## Esempi

Mostra come iterare su tutti i task di un progetto come una semplice lista.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


