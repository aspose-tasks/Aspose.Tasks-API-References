---
title: "TreeAlgorithmBase1.Alg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TreeAlgorithmBase. Procesa un nodo de un árbol"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/treealgorithmbase-1/alg/
---
## TreeAlgorithmBase&lt;T&gt;.Alg method

Procesa un nodo de un árbol.

```csharp
public abstract void Alg(T el, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | Nodo a procesar. |
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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


