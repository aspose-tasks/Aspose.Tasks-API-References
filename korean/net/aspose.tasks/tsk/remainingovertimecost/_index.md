---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 대한 남은 예정 초과 근무 비용입니다."
type: docs
weight: 970
url: /ko/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

작업에 대한 남은 예정 초과 근무 비용.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## 예제

Tsk.RemainingOvertimeCost 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


