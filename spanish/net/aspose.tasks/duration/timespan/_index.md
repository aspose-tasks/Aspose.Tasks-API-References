---
title: "Duration.TimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Duration. Obtiene la instancia TimeSpan de este objeto Duration. La instancia TimeSpan de este objeto Duration"
type: docs
weight: 40
url: /es/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Obtiene la instancia `TimeSpan` de este objeto Duration. La instancia TimeSpan de este objeto Duration.

```csharp
public TimeSpan TimeSpan { get; }
```

## Ejemplos

Muestra cómo convertir una duración a un TimeSpan.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// obtener la duración de la tarea
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


