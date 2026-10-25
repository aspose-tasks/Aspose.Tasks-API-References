---
title: "SplitPartCollection.Item"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SplitPartCollection. Возвращает часть разделения задачи по заданному индексу"
type: docs
weight: 20
url: /ru/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Извлекает часть задачи по заданному индексу.

```csharp
public SplitPart this[int index] { get; set; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс части. |

### Возвращаемое значение

часть разделения.

## Примечания

Индекс начинается с нуля. Возвращает null, если индекс находится за пределами массива.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


