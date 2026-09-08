---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 하위 작업 Gantt 막대에 대한 정보가 요약 작업 막대로 집계될지 여부를 결정합니다."
type: docs
weight: 690
url: /ko/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

하위 작업 간트 바에 대한 정보가 요약 작업 바로 집계되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## 예제

Tsk.IsRollup 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


