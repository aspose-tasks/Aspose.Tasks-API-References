---
title: "Sınıf TimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TimephasedData sınıfı. Zaman aşamalı bir veriyi temsil eder"
type: docs
weight: 2590
url: /tr/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

Zaman aşamalı bir veriyi temsil eder.

```csharp
public class TimephasedData
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TimephasedData](timephaseddata/)() | `TimephasedData` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | Zaman aşamalı veri dönemi için bitiş tarihini alır veya ayarlar. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | Zaman aşamalı veri dönemi için başlangıç tarihini alır veya ayarlar. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | Zaman aşamalı verinin tipini alır veya ayarlar. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | Zaman aşamalı verinin benzersiz tanımlayıcısını alır veya ayarlar |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | Zaman aşamalı veri dönemi için zaman birimini alır veya ayarlar. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | Zaman aşamalı veri dönemi için birim zaman başına değeri alır veya ayarlar. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | Bu nesnenin string değerini temsil eden Double örneğini alır. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | Bu nesnenin string değerini temsil eden TimeSpan örneğini alır. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | Birim tabanlı zaman aşamalı veri için bu nesnenin string değerini temsil eden Double örneğini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | Maliyet tabanlı zaman aşamalı veri için `TimephasedData` sınıfının yeni bir örneğini oluşturur ve başlatır. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | Maliyet tabanlı zaman aşamalı veri için `TimephasedData` sınıfının yeni bir örneğini oluşturur ve başlatır. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | Bir malzeme kaynağının atamasının birim tabanlı zaman aşamalı verisi için `TimephasedData` sınıfının yeni bir örneğini oluşturur ve başlatır. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | İş tabanlı zaman aşamalı veriler için `TimephasedData` sınıfının yeni bir örneğini oluşturur ve başlatır. |

## Örnekler

Özel zaman aşamalı verilerle nasıl çalışılacağını gösterir.

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

// özel zaman aşamalı tds ekleyelim
workAssignment.TimephasedData.Clear();

// çalışma günleri ekle
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// hafta sonu ekle
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

// çalışma günleri ekle
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// hafta sonu ekle
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


