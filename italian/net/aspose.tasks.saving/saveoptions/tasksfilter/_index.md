---
title: SaveOptions.TasksFilter
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: SaveOptions proprietà. Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt Foglio attività e Utilizzo attività.
type: docs
weight: 190
url: /it/net/aspose.tasks.saving/saveoptions/tasksfilter/
---
## SaveOptions.TasksFilter property

Ottiene o imposta la condizione utilizzata per filtrare le attività visualizzate nei diagrammi Gantt, Foglio attività e Utilizzo attività.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

### Osservazioni

Se il valore non è specificato, viene utilizzato il filtro predefinito che rimuove le attività non visibili, ovvero le attività discendenti delle attività compresse.

### Guarda anche

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SaveOptions](../)
* spazio dei nomi [Aspose.Tasks.Saving](../../saveoptions/)
* assemblea [Aspose.Tasks](../../../)


