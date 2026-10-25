---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 리소스 레벨링으로 인해 작업이 조기 시작일에서 지연되는 시간"
type: docs
weight: 770
url: /ko/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

리소스 레벨링으로 인해 작업이 초기 시작 날짜로부터 지연되는 시간.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## 예제

Tsk.LevelingDelay 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


