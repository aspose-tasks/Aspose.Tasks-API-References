---
title: "OutlineMaskCollection.RemoveAt"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineMaskCollection yöntemi. Belirtilen konumdaki bir öğeyi kaldırır"
type: docs
weight: 120
url: /tr/net/aspose.tasks/outlinemaskcollection/removeat/
---
## OutlineMaskCollection.RemoveAt method

Belirtilen dizindeki bir öğeyi kaldırır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Bir öğenin kaldırılacağı belirtilen sıfır tabanlı indeks. |

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

* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


