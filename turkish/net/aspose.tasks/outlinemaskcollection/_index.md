---
title: "Sınıf OutlineMaskCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineMaskCollection sınıfı. OutlineMask nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 1200
url: /tr/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

[`OutlineMask`](../outlinemask/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


