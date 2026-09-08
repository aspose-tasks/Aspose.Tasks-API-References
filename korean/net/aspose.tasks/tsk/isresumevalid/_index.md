---
title: "Tsk.IsResumeValid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업을 재개할 수 있는지 여부를 결정합니다"
type: docs
weight: 680
url: /ko/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

작업을 재개할 수 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## 예제

Tsk.IsResumeValid 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


