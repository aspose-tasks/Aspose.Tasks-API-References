---
title: "TaskBaseline.CompareTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskBaseline. Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado"
type: docs
weight: 90
url: /es/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Implementación de la interfaz IComparable. Compara esta instancia con el objeto Baseline especificado.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | TaskBaseline | el objeto Baseline especificado con el que comparar esta instancia. |

### Valor devuelto

devuelve -1 si esta instancia es menor que el objeto especificado, 1 si esta instancia es mayor que el objeto especificado; de lo contrario, devuelve 0.

## Ejemplos

Muestra cómo comprobar la igualdad de líneas base.

```csharp
var project = new Project();

// creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// mostrar duración de la línea base de la tarea
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// la igualdad de líneas base se verifica contra los números de la línea base.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Ver también

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


