---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。返回实例 TimephasedDataCollection 类，其中包含在指定 TimePhasedDataType 的给定开始和结束日期内的 TimephasedData 类实例。"
type: docs
weight: 720
url: /zh/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

返回实例 [`TimephasedDataCollection`](../../timephaseddatacollection/) 类，其中包含在指定 [`TimephasedDataType`](../../timephaseddatatype/) 的给定开始和结束日期内的 [`TimephasedData`](../timephaseddata/) 类实例。

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 时间分段数据的开始日期。 |
| 结束 | DateTime | 时间分段数据的结束日期。 |
| timephasedType | TimephasedDataType | 时间分段数据的类型（[`TimephasedDataType`](../../timephaseddatatype/)）。 |

### 返回值

返回一个列表，其中包含 [`TimephasedData`](../../timephaseddata/) 类的实例。

## 示例

展示如何在日期范围内生成资源分配的时间分段数据。

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// 设置项目属性
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// 创建资源分配
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// 设置 Backloaded 轮廓，它会将任务持续时间从 6 天增加到 10 天
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// 获取时间分段数据
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

返回包含在 AssignmentWork 的给定开始和结束日期内的 [`TimephasedData`](../timephaseddata/) 类实例的 [`TimephasedDataCollection`](../../timephaseddatacollection/) 对象。

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 时间分段数据的开始日期。 |
| 结束 | DateTime | 时间分段数据的结束日期。 |

### 返回值

返回一个列表，包含 [`TimephasedData`](../../timephaseddata/) 类的实例。

## 示例

展示如何在日期范围内生成资源分配的时间分段数据。

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// 设置项目属性
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// 创建资源分配
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);

// 设置 Backloaded 轮廓，它会将任务持续时间从 6 天增加到 10 天
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// 获取时间分段数据
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


