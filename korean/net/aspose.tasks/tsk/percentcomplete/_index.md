---
title: "Tsk.PercentComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 기간 중 완료된 비율로 표현된 작업의 현재 상태"
type: docs
weight: 880
url: /ko/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

작업의 현재 상태로, 작업 기간 중 완료된 비율로 표시됩니다.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## 예제

작업 퍼센트 완료를 업데이트하여 작업 진행률을 변경하는 방법을 보여줍니다.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// 작업에 접근하고 완료 비율을 표시합니다
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


