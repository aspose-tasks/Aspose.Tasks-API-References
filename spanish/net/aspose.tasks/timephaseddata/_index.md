---
title: "Clase TimephasedData"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TimephasedData. Representa un dato con fases de tiempo"
type: docs
weight: 2590
url: /es/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Representa datos con fases de tiempo.

```csharp
public class TimephasedData
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Inicializa una nueva instancia de la clase `TimephasedData`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Obtiene o establece la fecha de finalización de un período de datos con fases de tiempo. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Obtiene o establece la fecha de inicio de un período de datos con fases de tiempo. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Obtiene o establece el tipo de un dato con fases de tiempo. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Obtiene o establece el identificador único de un dato con fases de tiempo |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Obtiene o establece la unidad de tiempo de un período de datos con fases de tiempo. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Obtiene o establece el valor por unidad de tiempo para un período de datos con fases de tiempo. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Obtiene una instancia Double que representa el valor de cadena de este objeto. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Obtiene una instancia TimeSpan que representa el valor de cadena de este objeto. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Obtiene una instancia Double que representa el valor de cadena de este objeto para datos con fases de tiempo basados en unidades. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Crea e inicializa una nueva instancia de la clase `TimephasedData` para datos con fases de tiempo basados en costos. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Crea e inicializa una nueva instancia de la clase `TimephasedData` para datos con fases de tiempo basados en costos. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Crea e inicializa una nueva instancia de la clase `TimephasedData` para datos con fases de tiempo basados en unidades de una asignación de un recurso material. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Crea e inicializa una nueva instancia de la clase `TimephasedData` para datos de tiempo fase basados en trabajo. |

## Ejemplos

Muestra cómo trabajar con datos personalizados con fases de tiempo.

```csharp
var project = new Project(DataDir + "Project1.mpp") { CalculationMode = CalculationMode.None };

var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2018, 1, 1, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

var workAssignment = project.ResourceAssignments.Add(task, workResource);
workAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);
var costAssignment = project.ResourceAssignments.Add(task, costResource);
costAssignment.Set(Asn.WorkContour, WorkContourType.Contoured);

// agreguemos tds personalizados con fases de tiempo
workAssignment.TimephasedData.Clear();

// agregar días laborables
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// agregar fin de semana
var td2 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    TimeSpan.Zero,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

workAssignment.TimephasedData.Add(td1);
workAssignment.TimephasedData.Add(td2);

costAssignment.TimephasedData.Clear();

// agregar días laborables
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// agregar fin de semana
var td22 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 6, 8, 0, 0),
    new DateTime(2018, 1, 8, 8, 0, 0),
    0,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

costAssignment.TimephasedData.Add(td11);
costAssignment.TimephasedData.Add(td22);

Console.WriteLine("Print assignment timephased data:");
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
    foreach (var tds in assignment.TimephasedData)
    {
        Console.WriteLine("  Uid: " + tds.Uid);
        Console.WriteLine("  Start: " + tds.Start);
        Console.WriteLine("  Finish: " + tds.Finish);
        Console.WriteLine("  Type: " + tds.TimephasedDataType);
        Console.WriteLine("  Unit: " + tds.Unit);
        Console.WriteLine("  Value: " + tds.Value);
        Console.WriteLine("  ValueToCost: " + tds.ValueToCost);
        Console.WriteLine("  ValueToDuration: " + tds.ValueToDuration);
        Console.WriteLine("  ValueToUnits: " + tds.ValueToUnits);
        Console.WriteLine();
    }
}

project.Recalculate();
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


