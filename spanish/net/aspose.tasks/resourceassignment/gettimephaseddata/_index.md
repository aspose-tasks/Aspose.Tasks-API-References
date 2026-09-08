---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignment. Devuelve la instancia de la clase TimephasedDataCollection que contiene instancias de la clase TimephasedData dentro de las fechas de inicio y fin especificadas del TimephasedDataType especificado."
type: docs
weight: 720
url: /es/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Devuelve la instancia de la clase [`TimephasedDataCollection`](../../timephaseddatacollection/) que contiene instancias de la clase [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas del [`TimephasedDataType`](../../timephaseddatatype/) especificado.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio para los datos de tiempo faseado. |
| fin | DateTime | La fecha de fin para los datos de tiempo faseado. |
| timephasedType | TimephasedDataType | El tipo de datos de tiempo faseado ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Valor devuelto

devuelve una lista que contiene instancias de la clase [`TimephasedData`](../../timephaseddata/).

## Ejemplos

Muestra cómo generar datos con fases de tiempo de una asignación de recursos dentro de un rango de fechas.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Establecer propiedades del proyecto
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

// Establecer contorno Backloaded, aumenta la duración de la tarea de 6 a 10 días
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// obtener datos con fases de tiempo
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Devuelve el objeto [`TimephasedDataCollection`](../../timephaseddatacollection/) con las instancias de la clase [`TimephasedData`](../timephaseddata/) dentro de las fechas de inicio y fin dadas de AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | La fecha de inicio para los datos de tiempo faseado. |
| fin | DateTime | La fecha de fin para los datos de tiempo faseado. |

### Valor devuelto

devuelve una lista que contiene instancias de la clase [`TimephasedData`](../../timephaseddata/).

## Ejemplos

Muestra cómo generar datos con fases de tiempo de una asignación de recursos dentro de un rango de fechas.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Establecer propiedades del proyecto
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

// Establecer contorno Backloaded, aumenta la duración de la tarea de 6 a 10 días
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// obtener datos con fases de tiempo
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### Ver también

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


