---
title: "ResourceAssignment.TimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ResourceAssignment. Obtiene o establece la instancia de la clase TimephasedDataCollection que contiene elementos de la clase TimephasedData"
type: docs
weight: 600
url: /es/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Obtiene o establece la instancia de la clase [`TimephasedDataCollection`](../../timephaseddatacollection/) que contiene elementos de la clase `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Ejemplos

Muestra cómo leer los datos temporales de una asignación de recurso.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Crear asignación de recursos
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// obtener datos con fases de tiempo
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


