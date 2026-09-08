---
title: "Tsk.RemainingDuration"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 미완성 부분을 완료하는 데 필요한 시간입니다."
type: docs
weight: 960
url: /ko/net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

작업의 미완성 부분을 완료하는 데 필요한 시간.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## 예제

Tsk.RemainingDuration 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


