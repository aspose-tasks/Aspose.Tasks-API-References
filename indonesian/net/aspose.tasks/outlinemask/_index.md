---
title: "Kelas OutlineMask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.OutlineMask. Mewakili empat elemen dari masker yang mendefinisikan format kode outline"
type: docs
weight: 1190
url: /id/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Mewakili empat elemen dari mask yang mendefinisikan format kode outline.

```csharp
public class OutlineMask
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [OutlineMask](outlinemask/)() | Menginisialisasi sebuah instance baru dari kelas `OutlineMask`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Mendapatkan atau mengatur panjang maksimum (dalam karakter) nilai kode outline. 0 jika panjang tidak didefinisikan. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Mendapatkan atau mengatur level sebuah masker. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Mendapatkan atau mengatur pemisah nilai kode. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Mendapatkan atau mengatur tipe masker. |

## Contoh

Menampilkan cara bekerja dengan masker outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// atur tipe masker
mask.Type = MaskType.Characters;

// atur pemisah nilai kode
mask.Separator = "/";

// atur level masker
mask.Level = 1;

// atur panjang maksimum (dalam karakter) nilai kode outline. 0 jika panjang tidak ditentukan.
mask.Length = 2;

// tambahkan masker ke definisi
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


