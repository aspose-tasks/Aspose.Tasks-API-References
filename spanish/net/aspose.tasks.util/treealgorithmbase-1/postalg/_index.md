---
title: "TreeAlgorithmBase1.PostAlg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TreeAlgorithmBase. Llamado después del procesamiento de un nodo de un árbol"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/treealgorithmbase-1/postalg/
---
## TreeAlgorithmBase&lt;T&gt;.PostAlg method

Llamado después del procesamiento de un nodo de un árbol.

```csharp
public virtual void PostAlg(T el, int level)
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


