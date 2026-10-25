---
title: "Resource.GetTimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 方法。返回此对象的 TimephasedDataCollection 类实例，其中包含在指定的 TimephasedDataType 的给定开始和结束日期范围内的 TimephasedData 值"
type: docs
weight: 850
url: /zh/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

返回此对象的 [`TimephasedDataCollection`](../../timephaseddatacollection/) 类实例，其中包含在指定的 [`TimephasedDataType`](../../timephaseddatatype/) 的给定开始和结束日期范围内的 [`TimephasedData`](../timephaseddata/) 值。

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

[`TimephasedData`](../timephaseddata/) 列表。

## 示例

展示如何读取工作/成本资源的时间分段数据。

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// 通过 ID 获取 Resource
var resource = project.Resources.GetByUid(1);

// 打印 ResourceWork 的时间分段数据
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// 打印 ResourceCost 的时间分段数据
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

返回此对象的 [`TimephasedDataCollection`](../../timephaseddatacollection/)，其中包含在给定开始和结束日期范围内的 [`TimephasedData`](../timephaseddata/) 值。

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 时间分段数据的开始日期。 |
| 结束 | DateTime | 时间分段数据的结束日期。 |

### 返回值

[`TimephasedData`](../../timephaseddata/) 列表。

## 示例

展示如何读取工作/成本资源的时间分段数据。

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// 通过 ID 获取 Resource
var resource = project.Resources.GetByUid(1);

// 打印 ResourceWork 的时间分段数据
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// 打印 ResourceCost 的时间分段数据
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


