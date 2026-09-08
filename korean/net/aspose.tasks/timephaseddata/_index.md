---
title: "클래스 TimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TimephasedData 클래스. 시간 단계 데이터를 나타냅니다."
type: docs
weight: 2590
url: /ko/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

시간 구간 데이터를 나타냅니다.

```csharp
public class TimephasedData
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TimephasedData](timephaseddata/)() | `TimephasedData` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | 시간 단계 데이터 기간의 종료 날짜를 가져오거나 설정합니다. |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | 시간 단계 데이터 기간의 시작 날짜를 가져오거나 설정합니다. |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | 시간 단계 데이터의 유형을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | 시간 단계 데이터의 고유 식별자를 가져오거나 설정합니다. |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | 시간 단계 데이터 기간의 시간 단위를 가져오거나 설정합니다. |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | 시간 단계 데이터 기간의 시간 단위당 값을 가져오거나 설정합니다. |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | 이 객체의 문자열 값을 나타내는 Double 인스턴스를 가져옵니다. |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | 이 객체의 문자열 값을 나타내는 TimeSpan 인스턴스를 가져옵니다. |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | 단위 기반 시간 단계 데이터에 대한 이 객체의 문자열 값을 나타내는 Double 인스턴스를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | 비용 기반 시간 단계 데이터에 대한 `TimephasedData` 클래스의 새 인스턴스를 생성하고 초기화합니다. |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | 비용 기반 시간 단계 데이터에 대한 `TimephasedData` 클래스의 새 인스턴스를 생성하고 초기화합니다. |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | 자재 리소스 할당의 단위 기반 시간 단계 데이터에 대한 `TimephasedData` 클래스의 새 인스턴스를 생성하고 초기화합니다. |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | `TimephasedData` 클래스를 사용하여 작업 기반 시간 단계 데이터를 위한 새 인스턴스를 생성하고 초기화합니다. |

## 예제

사용자 정의 시간 구간 데이터 작업 방법을 보여줍니다.

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

// 사용자 정의 시간 구간 tds를 추가합니다.
workAssignment.TimephasedData.Clear();

// 근무일 추가
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// 주말 추가
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

// 근무일 추가
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// 주말 추가
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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


