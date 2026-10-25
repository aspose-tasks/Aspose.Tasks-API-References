---
title: "Tsk.RemainingCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 남은 예정 작업을 완료하는 데 발생할 남은 예정 비용"
type: docs
weight: 950
url: /ko/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

남은 예정 작업을 완료하는 데 발생할 남은 예정 비용.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
```

## 예제

작업 비용을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();

// 작업을 추가하고 비용을 설정합니다.
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// 작업의 비용 관련 속성을 표시합니다.
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


