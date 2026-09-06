---
title: "枚举 BarItemType。"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.BarItemType 枚举。用于更改条形样式的项目类型。"
type: docs
weight: 2940
url: /zh/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

用于更改条形样式的项目类型。

```csharp
public enum BarItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Task | `0` | 表示任务条形项目类型。 |
| Summary | `1` | 表示汇总条形项目类型。 |
| ProjectSummary | `2` | 表示项目汇总条形项目类型。 |
| ManualTask | `3` | 表示手动任务条形项目类型。 |
| InactiveTask | `4` | 表示非活动任务条形项目类型。 |
| CriticalTask | `5` | 表示关键任务条形项目类型。 |
| Milestone | `6` | 表示里程碑任务条形项目类型。 |
| ManualSummary | `7` | 表示手动汇总条形项目类型。 |
| Split | `8` | 表示拆分条形项目类型。 |
| ExternalTasks | `9` | 表示外部任务条形项目类型。 |
| ExternalMilestone | `10` | 指示外部里程碑栏项目类型。 |
| Deadline | `11` | 指示截止日期栏项目类型。 |
| Progress | `12` | 指示进度栏项目类型。 |
| StartOnly | `13` | 指示仅开始栏项目类型。 |
| FinishOnly | `14` | 指示仅完成栏项目类型。 |
| DurationOnly | `15` | 指示仅持续时间栏项目类型。 |
| InactiveMilestone | `16` | 指示非活动里程碑栏项目类型。 |
| InactiveSummary | `17` | 指示非活动汇总栏项目类型。 |
| SummaryRollup | `18` | 汇总回滚栏项目类型。 |

## 示例

展示如何通过使用 &lt;see cref=\"Aspose.Tasks.Visualization.BarStyle\" /&gt;s 来自定义任务栏。

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


