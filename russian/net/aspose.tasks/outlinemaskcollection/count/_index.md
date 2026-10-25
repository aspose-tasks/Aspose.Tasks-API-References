---
title: "OutlineMaskCollection.Count"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineMaskCollection. Получает количество элементов, содержащихся в этой коллекции"
type: docs
weight: 10
url: /ru/net/aspose.tasks/outlinemaskcollection/count/
---
## OutlineMaskCollection.Count property

Получает количество элементов, содержащихся в этой коллекции.

```csharp
public int Count { get; }
```

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

* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


