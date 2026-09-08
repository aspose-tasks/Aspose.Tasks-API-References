---
title: "Clase CheckCircuit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.CheckCircuit. Verifica si un árbol de tareas contiene un circuito"
type: docs
weight: 2680
url: /es/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Comprueba si un árbol (de tareas) contiene un circuito.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Inicializa una nueva instancia de la clase `CheckCircuit`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Comprueba si el objeto especificado ya fue procesado. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


