---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. Microsoft Project에서 일정 충돌 경고 표시기를 숨길지 여부를 나타냅니다."
type: docs
weight: 540
url: /ko/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Microsoft Project에서 일정 충돌 경고 표시기를 숨길지 여부를 나타냅니다.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## 예제

Tsk.IgnoreWarnings 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


