---
title: "Tsk.Type"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 유형"
type: docs
weight: 1100
url: /ko/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

작업의 유형.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## 예제

Tsk.Type 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


