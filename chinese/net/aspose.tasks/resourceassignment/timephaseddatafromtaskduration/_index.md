---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。根据任务持续时间和计划开始日期生成时间分段数据列表"
type: docs
weight: 780
url: /zh/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

根据任务持续时间和计划开始日期生成分阶段数据列表。

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日历 | 日历 | 用于生成时间分段数据的日历。 |

## 示例

展示如何为任务添加拆分。

```csharp
var project = new Project();

// 获取标准日历
var calendar = project.Get(Prj.Calendar);

// 设置项目的日历设置
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// 向根任务添加新任务
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// 创建新的资源分配并生成时间分段数据
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// 将任务拆分为 3 部分。
// 为 SplitTask 方法提供开始日期和结束日期参数，以用于拆分
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### 另见

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


