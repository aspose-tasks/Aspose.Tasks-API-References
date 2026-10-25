---
title: "Tsk.ManualFinish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 수동으로 예약된 완료 시점을 정의합니다"
type: docs
weight: 790
url: /ko/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

작업의 수동으로 일정이 지정된 완료일을 정의합니다.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## 예제

Tsk.ManualFinish 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


