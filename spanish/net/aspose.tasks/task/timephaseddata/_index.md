---
title: "Task.TimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene o establece un objeto TimephasedDataCollection de esta tarea. El bloque de datos faseados asociado a una tarea"
type: docs
weight: 1220
url: /es/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Obtiene o establece un objeto TimephasedDataCollection de esta tarea. El bloque de datos faseados en el tiempo asociado a una tarea.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Observaciones

Lectura soportada solo para formato XML.

## Ejemplos

Muestra cómo iterar sobre los datos faseados de la tarea.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


