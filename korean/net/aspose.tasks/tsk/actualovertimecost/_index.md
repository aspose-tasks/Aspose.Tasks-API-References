---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 할당된 리소스가 작업에 대해 이미 수행한 초과 근무에 발생한 비용"
type: docs
weight: 50
url: /ko/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용이 발생합니다.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## 예제

Tsk.ActualOvertimeCost 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


