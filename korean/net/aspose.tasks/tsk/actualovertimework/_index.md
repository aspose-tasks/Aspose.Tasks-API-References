---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 할당된 리소스가 이미 수행한 실제 초과 근무량"
type: docs
weight: 60
url: /ko/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

작업에 할당된 리소스가 이미 수행한 초과 근무량.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## 예제

Tsk.ActualOvertimeWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


