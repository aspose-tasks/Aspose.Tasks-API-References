---
title: "Tsk.IsExpanded"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. GanttChart 보기에서 요약 작업이 확장되었는지 여부를 결정합니다"
type: docs
weight: 590
url: /ko/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

간트 차트 보기에서 요약 작업이 확장되어 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## 예제

Shows how to read/write Tsk.IsExpanded property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


