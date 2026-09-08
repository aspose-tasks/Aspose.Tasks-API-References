---
title: "SplitPartCollection.ToArray"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод SplitPartCollection. Копирует все части из коллекции в новый массив"
type: docs
weight: 40
url: /ru/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Копирует все части из коллекции в новый массив.

```csharp
public SplitPart[] ToArray()
```

### Возвращаемое значение

Массив объектов [`SplitPart`](../../splitpart/).

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


