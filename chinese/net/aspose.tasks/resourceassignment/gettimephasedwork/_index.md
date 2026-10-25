---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。获取指定日期时间间隔的分阶段工作量"
type: docs
weight: 730
url: /zh/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

获取指定日期时间间隔的分阶段工作量。

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 日期时间间隔的开始。 |
| 结束 | DateTime | 日期时间间隔的结束。 |
| timephasedDataType | TimephasedDataType | 要使用的分阶段数据类型。 |

## 示例

展示如何计算任意日期时间间隔的分配工作量。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// 打印每小时的分配工作量。
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### 另见

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

获取指定日期时间间隔的分阶段工作量。

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 日期时间间隔的开始。 |
| 结束 | DateTime | 日期时间间隔的结束。 |

### 另见

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


