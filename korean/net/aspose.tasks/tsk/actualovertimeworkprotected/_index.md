---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 실제 초과 근무가 보호되는 기간"
type: docs
weight: 70
url: /ko/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

실제 초과 근무가 보호되는 기간.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## 예제

Tsk.ActualOvertimeWorkProtected 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


