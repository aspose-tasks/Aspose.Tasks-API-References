---
title: "Enum MaskType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MaskType enum. Bir maskenin türünü belirtir."
type: docs
weight: 1000
url: /tr/net/aspose.tasks/masktype/
---
## MaskType enumeration

Bir maskenin türünü belirtir.

```csharp
public enum MaskType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Null | `0` | Null maske türünü gösterir. |
| Numbers | `1` | Sayılar maske türünü gösterir. |
| UpperCaseLetters | `2` | UpperCaseLetters maske türünü gösterir. |
| LowerCaseLetters | `3` | LowerCaseLetters maske türünü gösterir. |
| Characters | `4` | Characters maske türünü gösterir. |
| Val4 | `5` | Lookup for Cost maske türünü gösterir. |
| Val5 | `6` | Lookup for Dates maske türünü gösterir. |
| Val6 | `7` | Lookup for Durations maske türünü gösterir. |
| Val7 | `8` | Lookup for Numbers maske türünü gösterir. |
| Val8 | `9` | Lookup for Flags maske türünü gösterir. |
| Val9 | `10` | Lookup for FinishDate maske türünü gösterir. |

## Örnekler

Outline maske koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// ana hat maskelerini temizle
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

// yanlış bir maske ekle.
outline.Masks.Insert(0, maskWrong);

// koleksiyonun indeks erişimini kullanarak maskeyi düzenle.
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// indeks ile yanlış bir maskeyi kaldır.
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// maskeler üzerinde yinele.
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


