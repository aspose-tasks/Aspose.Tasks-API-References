---
title: "Tsk.IsSummary"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업이 요약 작업인지 여부를 결정합니다"
type: docs
weight: 720
url: /ko/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

작업이 요약 작업인지 여부를 결정합니다.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## 예제

Tsk.IsSummary 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


