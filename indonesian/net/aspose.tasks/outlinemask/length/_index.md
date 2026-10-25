---
title: "OutlineMask.Length"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineMask. Mendapatkan atau mengatur panjang maksimum dalam karakter dari nilai kode outline. 0 jika panjang tidak didefinisikan"
type: docs
weight: 20
url: /id/net/aspose.tasks/outlinemask/length/
---
## OutlineMask.Length property

Mendapatkan atau mengatur panjang maksimum (dalam karakter) nilai kode outline. 0 jika panjang tidak didefinisikan.

```csharp
public int Length { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


