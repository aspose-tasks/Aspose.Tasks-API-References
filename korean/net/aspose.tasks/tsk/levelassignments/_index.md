---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 레벨링 기능이 과다 할당을 해결하기 위해 개별 할당을 지연시키고 분할할 수 있는지 여부를 결정합니다."
type: docs
weight: 750
url: /ko/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

레벨링 기능이 과다 할당을 해결하기 위해 개별 할당을 지연시키고 분할할 수 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## 예제

Tsk.LevelAssignments 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


