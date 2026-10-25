---
title: "ResourceAssignment.MakeTPs"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment método. Genera una lista de datos con fase temporal"
type: docs
weight: 740
url: /es/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Genera una lista de datos por fases de tiempo.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio especificada. |
| tiempo | TimeSpan | El tiempo de trabajo especificado. |
| calendario | Calendar | El calendario de trabajo especificado. |
| lista | List`1 | La lista de datos con fase temporal. |
| isWorking | Boolean | La bandera especificada que indica si los datos con fase temporal están en funcionamiento o no. |
| tipo | Int32 | El tipo de datos con fase temporal especificado. |

### Valor devuelto

Una fecha máxima de la lista o la fecha de inicio si la lista está vacía.

## Ejemplos

Muestra cómo generar TPs mediante parámetros.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### Ver también

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


