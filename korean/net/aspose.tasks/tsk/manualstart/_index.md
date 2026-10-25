---
title: "Tsk.ManualStart"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 수동으로 예약된 시작을 정의합니다."
type: docs
weight: 800
url: /ko/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

작업의 수동으로 일정이 지정된 시작일을 정의합니다.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## 예제

Tsk.ManualStart 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


