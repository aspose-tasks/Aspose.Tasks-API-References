---
title: "Duration.TimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Duration. Получает экземпляр TimeSpan этого объекта Duration. Экземпляр TimeSpan этого объекта Duration"
type: docs
weight: 40
url: /ru/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

Получает экземпляр `TimeSpan` этого объекта Duration. Экземпляр TimeSpan этого объекта Duration.

```csharp
public TimeSpan TimeSpan { get; }
```

## Примеры

Показывает, как преобразовать длительность в TimeSpan.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// получить длительность задачи
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


