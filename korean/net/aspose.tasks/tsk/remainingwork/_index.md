---
title: "Tsk.RemainingWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 또는 작업 집합을 완료하는 데 아직 필요한 시간을 나타냅니다."
type: docs
weight: 990
url: /ko/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

작업 또는 작업 집합을 완료하는 데 아직 필요한 시간.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## 예제

Tsk.RemainingWork 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


