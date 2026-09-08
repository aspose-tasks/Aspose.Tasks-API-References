---
title: "Tsk.PhysicalPercentComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 수행된 작업의 예산 비용(BCWP) 계산의 대안으로 사용할 수 있는 완료 비율 값"
type: docs
weight: 900
url: /ko/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

예산 작업 수행 비용(BCWP)을 계산하기 위한 대안으로 사용할 수 있는 완료 퍼센트 값.

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## 예제

Tsk.PhysicalPercentComplete 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


