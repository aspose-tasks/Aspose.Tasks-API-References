---
title: "Tsk.DisplayOnTimeline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업을 타임라인 보기에서 표시할지 여부를 지정합니다."
type: docs
weight: 290
url: /ko/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

작업을 타임라인 보기에서 표시할지 여부를 지정합니다.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## 예제

Tsk.DisplayOnTimeline 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


