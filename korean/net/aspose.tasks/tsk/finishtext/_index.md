---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 종료 텍스트를 반환합니다."
type: docs
weight: 410
url: /ko/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

작업의 종료 텍스트를 반환합니다.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## 예제

Tsk.FinishText 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


