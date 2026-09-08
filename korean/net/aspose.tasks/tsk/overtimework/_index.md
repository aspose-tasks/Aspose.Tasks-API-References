---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 할당된 모든 리소스가 수행하도록 예정된 초과 근무량을 나타냅니다."
type: docs
weight: 870
url: /ko/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

작업에 할당된 모든 리소스가 수행하도록 예정된 초과 근무량.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


