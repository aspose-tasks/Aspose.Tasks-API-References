---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 기간 텍스트를 반환합니다."
type: docs
weight: 310
url: /ko/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

작업의 기간 텍스트를 반환합니다.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## 예제

Tsk.DurationText 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


