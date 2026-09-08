---
title: "CheckCircuit.CheckCircuit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de CheckCircuit. Inicializa una nueva instancia de la clase CheckCircuit"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Inicializa una nueva instancia de la clase [`CheckCircuit`](../).

```csharp
public CheckCircuit()
```

## Ejemplos

Muestra cómo detectar la estructura rota del proyecto.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// verificar la estructura del proyecto.
// Se lanzará el <see cref="TasksException"> si la estructura del proyecto es incorrecta.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Ver también

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


