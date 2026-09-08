---
title: "Класс SplitPartCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.SplitPartCollection. Коллекция, представляющая части задачи."
type: docs
weight: 2300
url: /ru/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Коллекция, представляющая части задачи.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Получает количество частей в коллекции. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Извлекает часть задачи по заданному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Копирует все части из коллекции в новый массив. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


