---
title: "TaskBaseline.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskBaseline. Devuelve un valor de código hash para la instancia de la clase TaskBaseline."
type: docs
weight: 110
url: /es/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener el código hash de un baseline de tarea.

```csharp
var project = new Project();

// creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// mostrar duración de la línea base de la tarea
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// el código hash de un calendario es igual al número de baseline 
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Ver también

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


