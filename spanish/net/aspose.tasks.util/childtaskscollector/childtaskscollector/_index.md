---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de ChildTasksCollector. Inicializa una nueva instancia de la clase ChildTasksCollector"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Inicializa una nueva instancia de la clase [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
```

## Ejemplos

Muestra cómo iterar sobre todas las tareas en un proyecto como una lista simple.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizar todas las tareas recopiladas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Ver también

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


