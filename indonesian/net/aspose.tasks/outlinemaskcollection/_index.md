---
title: "Kelas OutlineMaskCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.OutlineMaskCollection class. Mewakili sekumpulan objek OutlineMask"
type: docs
weight: 1200
url: /id/net/aspose.tasks/outlinemaskcollection/
---
## OutlineMaskCollection class

Mewakili sekumpulan objek [`OutlineMask`](../outlinemask/).

```csharp
public class OutlineMaskCollection : IList<OutlineMask>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/outlinemaskcollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/outlinemaskcollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [Item](../../aspose.tasks/outlinemaskcollection/item/) { get; set; } | Mengembalikan atau mengatur elemen pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/outlinemaskcollection/add/)(OutlineMask) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/outlinemaskcollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/outlinemaskcollection/contains/)(OutlineMask) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/outlinemaskcollection/copyto/)(OutlineMask[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/outlinemaskcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [IndexOf](../../aspose.tasks/outlinemaskcollection/indexof/)(OutlineMask) | Menentukan indeks dari item yang ditentukan dalam koleksi ini. |
| [Insert](../../aspose.tasks/outlinemaskcollection/insert/)(int, OutlineMask) | Menyisipkan item yang ditentukan pada indeks yang ditentukan. |
| [Remove](../../aspose.tasks/outlinemaskcollection/remove/)(OutlineMask) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [RemoveAt](../../aspose.tasks/outlinemaskcollection/removeat/)(int) | Menghapus sebuah item pada indeks yang ditentukan. |

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

* class [OutlineMask](../outlinemask/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


