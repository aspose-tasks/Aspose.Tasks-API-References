---
title: "열거형 BarItemType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.BarItemType 열거형. 막대 스타일을 변경할 항목 유형"
type: docs
weight: 2940
url: /ko/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

막대 스타일을 변경할 항목 유형입니다.

```csharp
public enum BarItemType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Task | `0` | 작업 막대 항목 유형을 나타냅니다. |
| Summary | `1` | 요약 막대 항목 유형을 나타냅니다. |
| ProjectSummary | `2` | 프로젝트 요약 막대 항목 유형을 나타냅니다. |
| ManualTask | `3` | 수동 작업 막대 항목 유형을 나타냅니다. |
| InactiveTask | `4` | 비활성 작업 막대 항목 유형을 나타냅니다. |
| CriticalTask | `5` | 중요 작업 막대 항목 유형을 나타냅니다. |
| Milestone | `6` | 마일스톤 작업 막대 항목 유형을 나타냅니다. |
| ManualSummary | `7` | 수동 요약 막대 항목 유형을 나타냅니다. |
| Split | `8` | 분할 막대 항목 유형을 나타냅니다. |
| ExternalTasks | `9` | 외부 작업 막대 항목 유형을 나타냅니다. |
| ExternalMilestone | `10` | 외부 마일스톤 막대 항목 유형을 나타냅니다. |
| Deadline | `11` | 마감일 막대 항목 유형을 나타냅니다. |
| Progress | `12` | 진행 막대 항목 유형을 나타냅니다. |
| StartOnly | `13` | 시작 전용 막대 항목 유형을 나타냅니다. |
| FinishOnly | `14` | 완료 전용 막대 항목 유형을 나타냅니다. |
| DurationOnly | `15` | 기간 전용 막대 항목 유형을 나타냅니다. |
| InactiveMilestone | `16` | 비활성 마일스톤 막대 항목 유형을 나타냅니다. |
| InactiveSummary | `17` | 비활성 요약 막대 항목 유형을 나타냅니다. |
| SummaryRollup | `18` | 요약 롤업 막대 항목 유형. |

## 예제

작업 막대를 &lt;see cref="Aspose.Tasks.Visualization.BarStyle" /&gt;를 사용하여 사용자 지정하는 방법을 보여줍니다.

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

### 또 보기

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


