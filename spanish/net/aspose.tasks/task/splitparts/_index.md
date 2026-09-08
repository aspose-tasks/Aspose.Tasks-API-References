---
title: "Task.SplitParts"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene una colección SplitPart que representa las porciones de una tarea"
type: docs
weight: 1110
url: /es/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Obtiene una colección SplitPart que representa las porciones de una tarea.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Ejemplos

Muestra cómo mostrar las partes divididas de la tarea.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Acceder a la tarea 
var task = project.RootTask.Children.GetById(4);

// Mostrar partes divididas de la tarea
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Ver también

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


