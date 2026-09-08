---
title: "Tsk.IsManual"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업이 수동으로 일정이 잡혔는지 여부를 결정합니다"
type: docs
weight: 610
url: /ko/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

작업이 수동으로 일정이 지정되었는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## 예제

Tsk.IsManual 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


