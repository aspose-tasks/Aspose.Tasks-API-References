---
title: "OutlineValue.IsCollapsed"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti OutlineValue. Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai outline terlipat atau tidak."
type: docs
weight: 40
url: /id/net/aspose.tasks/outlinevalue/iscollapsed/
---
## OutlineValue.IsCollapsed property

Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai outline terlipat atau tidak.

```csharp
public bool IsCollapsed { get; set; }
```

## Catatan

Ini baru untuk properti MS Project 2010.

## Contoh

Menampilkan cara bekerja dengan nilai outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// buat nilai outline
var value = new OutlineValue();

// atur nilai sebenarnya
value.Value = "Text value 1";

// atur Id unik dari nilai kode outline dalam sebuah proyek
value.ValueId = 1;

// dapatkan GUID yang mengidentifikasi nilai ini di antara nilai lain dalam seluruh proyek
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// atur tipe kode outline
value.Type = OutlineValueType.Text;

// atur deskripsi nilai outline
value.Description = "Text value descr 1";

// atur nilai yang menunjukkan apakah nilai outline terlipat atau tidak
value.IsCollapsed = false;

// periksa id nilai induk
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// buat nilai outline dengan durasi
var value2 = new OutlineValue();

// atur nilai durasi
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// atur Id unik dari nilai kode outline dalam sebuah proyek
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Lihat Juga

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


