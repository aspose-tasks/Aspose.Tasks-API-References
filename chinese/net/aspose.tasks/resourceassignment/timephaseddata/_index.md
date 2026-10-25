---
title: "ResourceAssignment.TimephasedData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 属性。获取或设置包含 TimephasedData 类元素的 TimephasedDataCollection 类的实例"
type: docs
weight: 600
url: /zh/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

获取或设置 [`TimephasedDataCollection`](../../timephaseddatacollection/) 类的实例，该实例包含 `TimephasedData` 类的元素。

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## 示例

展示如何读取资源分配的分阶段时间数据。

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
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
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// 获取时间分段数据
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### 另见

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


