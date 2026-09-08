---
title: "Duration.ToString"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Duration. Возвращает строковое представление этого экземпляра."
type: docs
weight: 120
url: /ru/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Возвращает строковое представление этого экземпляра.

```csharp
public override string ToString()
```

### Возвращаемое значение

строковое представление этого экземпляра.

## Примеры

Показывает, как преобразовать длительность в строку.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// получить длительность задачи
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### См. также

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


