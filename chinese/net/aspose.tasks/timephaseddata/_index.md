---
title: "类 TimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TimephasedData 类。表示时间分段数据"
type: docs
weight: 2590
url: /zh/net/aspose.tasks/timephaseddata/
---
## TimephasedData class

表示时间分段数据。

```csharp
public class TimephasedData
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [TimephasedData](timephaseddata/)() | 初始化 `TimephasedData` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Finish](../../aspose.tasks/timephaseddata/finish/) { get; set; } | 获取或设置时间分段数据期间的结束日期。 |
| [Start](../../aspose.tasks/timephaseddata/start/) { get; set; } | 获取或设置时间分段数据期间的开始日期。 |
| [TimephasedDataType](../../aspose.tasks/timephaseddata/timephaseddatatype/) { get; set; } | 获取或设置时间分段数据的类型。 |
| [Uid](../../aspose.tasks/timephaseddata/uid/) { get; set; } | 获取或设置时间分段数据的唯一标识符 |
| [Unit](../../aspose.tasks/timephaseddata/unit/) { get; set; } | 获取或设置时间分段数据期间的时间单位。 |
| [Value](../../aspose.tasks/timephaseddata/value/) { get; set; } | 获取或设置时间分段数据期间每单位时间的值。 |
| [ValueToCost](../../aspose.tasks/timephaseddata/valuetocost/) { get; set; } | 获取表示此对象字符串值的 Double 实例。 |
| [ValueToDuration](../../aspose.tasks/timephaseddata/valuetoduration/) { get; } | 获取表示此对象字符串值的 TimeSpan 实例。 |
| [ValueToUnits](../../aspose.tasks/timephaseddata/valuetounits/) { get; } | 获取表示基于单位的时间分段数据的此对象字符串值的 Double 实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased)(int, DateTime, DateTime, double, TimephasedDataType) | 创建并初始化 `TimephasedData` 类的一个新实例，用于基于成本的时间分段数据。 |
| static [CreateCostTimephased](../../aspose.tasks/timephaseddata/createcosttimephased/#createcosttimephased_1)(int, DateTime, DateTime, double, TimeUnitType, TimephasedDataType) | 创建并初始化 `TimephasedData` 类的一个新实例，用于基于成本的时间分段数据。 |
| static [CreateUnitTimephased](../../aspose.tasks/timephaseddata/createunittimephased/)(int, DateTime, DateTime, double, TimephasedDataType) | 创建并初始化 `TimephasedData` 类的一个新实例，用于材料资源分配的基于单位的时间分段数据。 |
| static [CreateWorkTimephased](../../aspose.tasks/timephaseddata/createworktimephased/)(int, DateTime, DateTime, TimeSpan, TimeUnitType, TimephasedDataType) | 创建并初始化 `TimephasedData` 类的新实例，用于基于工作时间相位的数据。 |

## 示例

展示如何使用自定义时间分段数据。

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

// 让我们添加自定义时间分段 tds
workAssignment.TimephasedData.Clear();

// 添加工作日
var td1 = TimephasedData.CreateWorkTimephased(
    workAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    TimeSpan.FromHours(40),
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentRemainingWork);

// 添加周末
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

// 添加工作日
var td11 = TimephasedData.CreateCostTimephased(
    costAssignment.Get(Asn.Uid),
    new DateTime(2018, 1, 2, 8, 0, 0),
    new DateTime(2018, 1, 5, 17, 0, 0),
    1,
    TimeUnitType.Hour,
    TimephasedDataType.AssignmentCost);

// 添加周末
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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


