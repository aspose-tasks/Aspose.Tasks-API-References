---
title: "CheckCircuit.Alg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CheckCircuit. Verifica si el objeto especificado ya fue procesado"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Comprueba si el objeto especificado ya fue procesado.

```csharp
public override void Alg(Task el, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | Tarea | Objeto a procesar. |
| nivel | Int32 | Nivel del nodo del árbol. |

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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


