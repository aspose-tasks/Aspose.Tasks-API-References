---
title: "Duration.ToDouble"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Convierte el objeto Duration a un valor Double."
type: docs
weight: 110
url: /es/net/aspose.tasks/duration/todouble/
---
## Duration.ToDouble method

Convierte el objeto Duration a un valor Double.

```csharp
public double ToDouble()
```

### Valor devuelto

Valor convertido.

## Ejemplos

Muestra cómo convertir una duración en diferentes tipos de unidades de tiempo.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Obtén una tarea para calcular su duración en diferentes formatos
var task = project.RootTask.Children.GetById(1);

// Obtén la duración en Minutos, Días, Horas, Semanas y Meses
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


