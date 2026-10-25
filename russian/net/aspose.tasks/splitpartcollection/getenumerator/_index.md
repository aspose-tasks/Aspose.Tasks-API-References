---
title: "SplitPartCollection.GetEnumerator"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод SplitPartCollection. Возвращает перечислитель для этой коллекции"
type: docs
weight: 30
url: /ru/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Возвращает перечислитель для этой коллекции.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Возвращаемое значение

перечислитель для этой коллекции.

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


