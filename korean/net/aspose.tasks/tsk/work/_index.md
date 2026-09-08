---
title: "Tsk.Work"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 할당된 모든 리소스에 대해 작업에 예정된 총 시간"
type: docs
weight: 1150
url: /ko/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

할당된 모든 리소스에 대해 작업에 예정된 총 시간.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## 예제

Tsk.Work 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


