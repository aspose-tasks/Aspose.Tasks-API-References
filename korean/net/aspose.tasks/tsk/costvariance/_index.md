---
title: "Tsk.CostVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 리소스 또는 할당에 대한 기준 비용과 총 비용의 차이입니다."
type: docs
weight: 240
url: /ko/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

작업, 리소스 또는 할당에 대한 기준 비용과 총 비용 간의 차이.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


