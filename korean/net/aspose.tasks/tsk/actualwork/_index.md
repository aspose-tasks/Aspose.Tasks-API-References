---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업에 할당된 리소스가 이미 수행한 작업량"
type: docs
weight: 90
url: /ko/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

작업에 할당된 리소스가 이미 수행한 작업량.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## 예제

Tsk.ActualWork 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


