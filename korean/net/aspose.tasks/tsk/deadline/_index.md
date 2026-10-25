---
title: "Tsk.Deadline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업이 완료되어야 하는 목표 날짜를 나타냅니다."
type: docs
weight: 270
url: /ko/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

작업이 완료될 예정인 목표 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## 예제

Tsk.Deadline 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


