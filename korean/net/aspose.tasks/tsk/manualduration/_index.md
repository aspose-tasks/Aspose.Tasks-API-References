---
title: "Tsk.ManualDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 수동으로 예약된 기간을 정의합니다"
type: docs
weight: 780
url: /ko/net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

작업의 수동으로 일정이 지정된 기간을 정의합니다.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## 예제

Tsk.ManualDuration 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


