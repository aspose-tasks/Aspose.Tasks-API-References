---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 null 작업인지 여부를 결정합니다."
type: docs
weight: 640
url: /ko/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

작업이 널 작업인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## 예제

Tsk.IsNull 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


