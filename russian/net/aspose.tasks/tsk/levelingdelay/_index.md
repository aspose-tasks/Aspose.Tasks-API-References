---
title: "Tsk.LevelingDelay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, на которое задача должна быть отложена от её ранней даты начала из‑за выравнивания ресурсов"
type: docs
weight: 770
url: /ru/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

Время, на которое задача должна быть отложена от своей ранней даты начала из‑за выравнивания ресурсов.

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.LevelingDelay.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


