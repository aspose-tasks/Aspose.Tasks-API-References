---
title: "Tsk.StartText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 시작 텍스트를 반환합니다."
type: docs
weight: 1030
url: /ko/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

작업의 시작 텍스트를 반환합니다.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## 예제

Tsk.StartText 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


