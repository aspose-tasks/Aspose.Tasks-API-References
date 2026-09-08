---
title: "Класс OutlineMaskCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OutlineMaskCollection. Представляет коллекцию объектов OutlineMask"
type: docs
weight: 1200
url: /ru/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Представляет коллекцию объектов [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Определяет индекс указанного элемента в этой коллекции. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Вставляет указанный элемент в указанный индекс. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Удаляет элемент по указанному индексу. |

## Примеры

Показывает, как работать с коллекциями контурных масок.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// очистить маски контуров
if (outline.Masks.Count > 0)
{
    if (!outline.Masks.IsReadOnly)
    {
        outline.Masks.Clear();
    }
}

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
var maskWrong = new OutlineMask();
maskWrong.Type = MaskType.Null;

outline.Masks.Add(mask);

// вставить неправильную маску
outline.Masks.Insert(0, maskWrong);

// изменить маску, используя доступ по индексу к коллекции
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// удалить неправильную маску по индексу
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// перебрать маски
foreach (var outlineMask in outline.Masks)
{
    Console.WriteLine("Length: " + outlineMask.Length);
    Console.WriteLine("Level: " + outlineMask.Level);
    Console.WriteLine("Separator: " + outlineMask.Separator);
    Console.WriteLine("Type: " + outlineMask.Type);
}

var otherProject = new Project(DataDir + "OutlineValues2010.mpp");

var otherOutline = otherProject.OutlineCodes[0];

var masks = new OutlineMask[outline.Masks.Count];
outline.Masks.CopyTo(masks, 0);

foreach (var maskToAdd in masks)
{
    if (!otherOutline.Masks.Contains(maskToAdd))
    {
        otherOutline.Masks.Add(maskToAdd);
    }
}
```

### См. также

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


