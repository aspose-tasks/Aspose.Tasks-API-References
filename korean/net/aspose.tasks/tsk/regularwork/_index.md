---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스가 수행하도록 예정된 초과 근무가 아닌 작업의 총량"
type: docs
weight: 940
url: /ko/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

리소스가 수행하도록 예정된 비초과 근무 총량.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## 예제

Tsk.RegularWork 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


