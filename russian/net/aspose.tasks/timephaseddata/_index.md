---
title: "Класс TimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TimephasedData. Представляет данные, разбитые по времени"
type: docs
weight: 2590
url: /ru/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Представляет данные, разбитые по времени.

```csharp
public class TimephasedData
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TimephasedData](timephaseddata/)() | Инициализирует новый экземпляр класса `TimephasedData`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Получает или задает дату завершения периода данных, разбитых по времени. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Получает или задает дату начала периода данных, разбитых по времени. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Получает или задает тип данных, разбитых по времени. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Получает или задает уникальный идентификатор данных, разбитых по времени |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Получает или задает единицу измерения времени периода данных, разбитых по времени. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Получает или задает значение за единицу времени для периода данных, разбитых по времени. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Получает экземпляр Double, который представляет строковое значение этого объекта. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Получает экземпляр TimeSpan, который представляет строковое значение этого объекта. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Получает экземпляр Double, который представляет строковое значение этого объекта для данных, разбитых по времени на основе единиц. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Создает и инициализирует новый экземпляр класса `TimephasedData` для данных, разбитых по времени на основе стоимости. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Создает и инициализирует новый экземпляр класса `TimephasedData` для данных, разбитых по времени на основе стоимости. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Создает и инициализирует новый экземпляр класса `TimephasedData` для данных, разбитых по времени на основе единиц, связанных с назначением материального ресурса. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | Создает и инициализирует новый экземпляр класса `TimephasedData` для данных, основанных на рабочем времени. |

## Примеры

Показывает, как работать с пользовательскими данными с фазированием во времени.

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

// добавим пользовательские фазированные tds
workAssignment.TimephasedData.Clear();

// добавить рабочие дни
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// добавить выходные
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

// добавить рабочие дни
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// добавить выходные
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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


