---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。生成时间分段数据的列表"
type: docs
weight: 740
url: /zh/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

生成分阶段数据列表。

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 指定的开始日期。 |
| 时间 | TimeSpan | 指定的工作时间。 |
| 日历 | 日历 | 指定的工作日历。 |
| 列表 | List`1 | 时间分段数据的列表。 |
| isWorking | Boolean | 指定的标志，用于指示时间分段数据是否为工作状态。 |
| 类型 | Int32 | 指定的时间分段数据类型。 |

### 返回值

列表中的最大日期，若列表为空则为开始日期。

## 示例

展示如何通过参数生成 TP。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### 另见

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


