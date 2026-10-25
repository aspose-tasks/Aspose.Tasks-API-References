---
title: "Duration.ToString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Devuelve una representación en cadena de esta instancia"
type: docs
weight: 120
url: /es/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Devuelve una representación en cadena de esta instancia.

```csharp
public override string ToString()
```

### Valor devuelto

una representación en cadena de esta instancia.

## Ejemplos

Muestra cómo convertir una duración a una cadena.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// obtener la duración de la tarea
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


