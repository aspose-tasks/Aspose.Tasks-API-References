---
title: "OutlineMaskCollection.Contains"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode OutlineMaskCollection. Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini, jika tidak false"
type: docs
weight: 60
url: /id/net/aspose.tasks/outlinemaskcollection/contains/
---
## OutlineMaskCollection.Contains method

Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.

```csharp
public bool Contains(OutlineMask item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | OutlineMask | item yang ditentukan untuk dicari. |

### Nilai Kembali

true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.

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

* class [OutlineMask](../../outlinemask/)
* class [OutlineMaskCollection](../)
* namespace [Aspose.Tasks](../../outlinemaskcollection/)
* assembly [Aspose.Tasks](../../../)


