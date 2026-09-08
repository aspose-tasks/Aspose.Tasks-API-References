---
title: "Tsk.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 남은 예정 초과 근무 시간 양입니다."
type: docs
weight: 980
url: /ko/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

남은 예정 초과 근무 시간량.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## 예제

Tsk.RemainingOvertimeWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


