---
title: "Tsk.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 완료된 작업 비율을 백분율로 표현한 작업의 현재 상태를 나타냅니다."
type: docs
weight: 890
url: /ko/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

작업의 현재 상태를 완료된 작업 비율로 표시합니다.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## 예제

Tsk.PercentWorkComplete 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


