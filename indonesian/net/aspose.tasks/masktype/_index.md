---
title: "Enum MaskType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.MaskType. Menentukan jenis masker"
type: docs
weight: 1000
url: /id/net/aspose.tasks/masktype/
---
## MaskType enumeration

Menentukan tipe sebuah masker.

```csharp
public enum MaskType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Null | `0` | Menunjukkan jenis masker Null. |
| Numbers | `1` | Menunjukkan jenis masker Numbers. |
| UpperCaseLetters | `2` | Menunjukkan jenis masker UpperCaseLetters. |
| LowerCaseLetters | `3` | Menunjukkan jenis masker LowerCaseLetters. |
| Characters | `4` | Menunjukkan jenis masker Characters. |
| Val4 | `5` | Menunjukkan jenis masker Lookup untuk Cost. |
| Val5 | `6` | Menunjukkan jenis masker Lookup untuk Dates. |
| Val6 | `7` | Menunjukkan jenis masker Lookup untuk Durations. |
| Val7 | `8` | Menunjukkan jenis masker Lookup untuk Numbers. |
| Val8 | `9` | Menunjukkan jenis masker Lookup untuk Flags. |
| Val9 | `10` | Menunjukkan jenis masker Lookup untuk FinishDate. |

## Contoh

Menampilkan cara bekerja dengan koleksi masker outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = project.OutlineCodes[0];

// hapus mask outline
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

// menyisipkan masker yang salah
outline.Masks.Insert(0, maskWrong);

// mengedit masker dengan menggunakan akses indeks koleksi
var idx = outline.Masks.IndexOf(mask);
outline.Masks[idx].Length = 2;

// menghapus masker yang salah dengan indeks
var idxOfWrong = outline.Masks.IndexOf(maskWrong);
outline.Masks.RemoveAt(idxOfWrong);

// mengiterasi masker
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

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


