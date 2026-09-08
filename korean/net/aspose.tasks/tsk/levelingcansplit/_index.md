---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스 레벨링 기능이 이 작업의 남은 작업을 분할할 수 있는지 여부를 결정합니다."
type: docs
weight: 760
url: /ko/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

리소스 레벨링 기능이 이 작업의 남은 작업을 분할시킬 수 있는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## 예제

Tsk.LevelingCanSplit 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


