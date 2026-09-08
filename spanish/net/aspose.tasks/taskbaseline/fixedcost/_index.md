---
title: "TaskBaseline.FixedCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskBaseline. Obtiene o establece un costo fijo de la tarea cuando se guardó el baseline."
type: docs
weight: 50
url: /es/net/aspose.tasks/taskbaseline/fixedcost/
---
## TaskBaseline.FixedCost property

Obtiene o establece un costo fijo de la tarea cuando se guardó la línea base.

```csharp
public double FixedCost { get; set; }
```

## Ejemplos

Muestra cómo obtener acceso a la información de la línea base.

```csharp
var project = new Project();

// Creando TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Mostrar duración de la línea base de la tarea
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// valor que indica si esta es una Línea Base Intermedia
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// imprimir datos temporales de la línea base de la tarea
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Ver también

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


