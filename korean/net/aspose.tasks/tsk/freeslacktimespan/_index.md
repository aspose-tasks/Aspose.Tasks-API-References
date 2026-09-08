---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 후속 작업을 지연시키지 않고 작업을 연기할 수 있는 시간입니다."
type: docs
weight: 450
url: /ko/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

후속 작업을 지연시키지 않고 작업을 지연시킬 수 있는 시간.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## 예제

Tsk.FreeSlackTimeSpan 속성을 읽는 방법을 보여줍니다. 이 속성은 계산되므로 일반적으로 명시적으로 설정할 필요가 없습니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


