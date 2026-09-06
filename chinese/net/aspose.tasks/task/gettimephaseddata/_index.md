---
title: "Task.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。返回 TimephasedDataCollection 对象，其中包含指定时间分段数据类型在给定开始和结束日期范围内的 TimephasedData 值。"
type: docs
weight: 1360
url: /zh/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

返回 [`TimephasedDataCollection`](../../timephaseddatacollection/) 对象，其中包含指定时间分段数据类型在给定开始和结束日期范围内的 [`TimephasedData`](../timephaseddata/) 值。

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

一个 [`TimephasedDataCollection`](../../timephaseddatacollection/) 对象，其中包含指定时间分段数据类型在给定开始和结束日期范围内的 [`TimephasedData`](../timephaseddata/) 值。

## 示例

展示如何获取任务的时间分段数据（特定类型）。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

返回 [`TimephasedDataCollection`](../../timephaseddatacollection/) 对象，其中包含在给定开始和结束日期范围内的 [`TimephasedData`](../timephaseddata/) 值。

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 时间分段数据的开始日期。 |
| 结束 | DateTime | 时间分段数据的结束日期。 |

### 返回值

列出需填写的[`TimephasedData`](../../timephaseddata/)。

## 示例

展示如何获取任务的时间分段数据（使用 TaskWork 类型）。

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


