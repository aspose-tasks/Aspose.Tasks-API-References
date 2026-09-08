---
title: "Перечисление MaskType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.MaskType. Указывает тип маски"
type: docs
weight: 1000
url: /ru/net/aspose.tasks/masktype/
---
## MaskType enumeration

Указывает тип маски.

```csharp
public enum MaskType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Null | `0` | Указывает тип маски Null. |
| Numbers | `1` | Указывает тип маски Numbers. |
| UpperCaseLetters | `2` | Указывает тип маски UpperCaseLetters. |
| LowerCaseLetters | `3` | Указывает тип маски LowerCaseLetters. |
| Characters | `4` | Указывает тип маски Characters. |
| Val4 | `5` | Указывает тип маски Lookup for Cost. |
| Val5 | `6` | Указывает тип маски Lookup for Dates. |
| Val6 | `7` | Указывает тип маски Lookup for Durations. |
| Val7 | `8` | Указывает тип маски Lookup for Numbers. |
| Val8 | `9` | Указывает тип маски Lookup for Flags. |
| Val9 | `10` | Указывает тип маски Lookup for FinishDate. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


