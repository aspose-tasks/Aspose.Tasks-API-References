---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스가 할당된 모든 작업 또는 리소스 할당에 대한 작업의 총 초과 근무 비용"
type: docs
weight: 860
url: /ko/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

작업에 대한 총 초과 근무 비용, 모든 할당된 작업에 대한 리소스의 비용, 또는 리소스 할당에 대한 비용.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
```

## 예제

작업 초과 근무를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// 작업의 초과 근무 및 완료 비율을 읽습니다
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // 완료 비율 설정
    task.Set(Tsk.PercentComplete, 100);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


