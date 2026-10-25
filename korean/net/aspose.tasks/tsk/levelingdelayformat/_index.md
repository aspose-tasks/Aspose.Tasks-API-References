---
title: "LevelingDelayFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "지연 기간을 표현하는 형식입니다."
type: docs
weight: 790
url: /ko/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

지연 기간을 표현하는 형식입니다.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### 예제

Tsk.LevelingDelayFormat 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Tasks.dll용으로 생성됨 -->
