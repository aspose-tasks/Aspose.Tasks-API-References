---
title: "SplitPart.Start"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SplitPart 속성. SplitPart의 시작 날짜를 가져옵니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/splitpart/start/
---
## SplitPart.Start property

SplitPart의 시작 날짜를 가져옵니다.

```csharp
public DateTime Start { get; }
```

## 예제

분할된 작업의 split part를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// 먼저 리소스 할당 시간 단계 데이터를 생성해야 합니다.
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// 작업을 분할합니다.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// 분할 부분을 반복합니다
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### 또 보기

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


