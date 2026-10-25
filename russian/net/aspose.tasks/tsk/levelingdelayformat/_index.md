---
title: "LevelingDelayFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Формат выражения длительности задержки."
type: docs
weight: 790
url: /ru/net/aspose.tasks/tsk/levelingdelayformat/
---
## Tsk.LevelingDelayFormat field

Формат выражения длительности задержки.

```csharp
public static readonly Key<TimeUnitType, TaskKey> LevelingDelayFormat;
```

### Примеры

Показывает, как читать/записывать свойство Tsk.LevelingDelayFormat.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelayFormat, TimeUnitType.Hour);

Console.WriteLine("Leveling Delay Format: " + task.Get(Tsk.LevelingDelayFormat));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2)
* enum [TimeUnitType](../../timeunittype)
* enum [TaskKey](../../taskkey)
* class [Tsk](../../tsk)
* namespace [Aspose.Tasks](../../tsk)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
