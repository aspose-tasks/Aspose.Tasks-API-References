---
title: "SplitPartCollection.Count"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SplitPartCollection. Возвращает количество частей в коллекции"
type: docs
weight: 10
url: /ru/net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

Получает количество частей в коллекции.

```csharp
public int Count { get; }
```

## Примеры

Показывает, как работать с коллекциями частей задачи.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// итерация по частям задачи
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// получить часть по индексу
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// выполнить некоторые действия с первой частью задачи
```

### См. также

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


