---
title: "Class OutlineValue"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.OutlineValue class. Mewakili nilai outline"
type: docs
weight: 1210
url: /id/net/aspose.tasks/outlinevalue/
---
## OutlineValue class

Mewakili nilai outline.

```csharp
public class OutlineValue
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [OutlineValue](outlinevalue/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Description](../../aspose.tasks/outlinevalue/description/) { get; set; } | Mendapatkan atau mengatur deskripsi nilai outline. |
| [DurationValue](../../aspose.tasks/outlinevalue/durationvalue/) { get; set; } | Mendapatkan atau mengatur durasi jika Tipe adalah Duration. |
| [IsCollapsed](../../aspose.tasks/outlinevalue/iscollapsed/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah nilai outline terlipat atau tidak. |
| [ParentValueId](../../aspose.tasks/outlinevalue/parentvalueid/) { get; set; } | Mendapatkan atau mengatur Id dari node induk kode outline. |
| [Type](../../aspose.tasks/outlinevalue/type/) { get; set; } | Mendapatkan atau mengatur tipe kode outline. |
| [Value](../../aspose.tasks/outlinevalue/value/) { get; set; } | Mendapatkan atau mengatur nilai aktual. |
| [ValueGuid](../../aspose.tasks/outlinevalue/valueguid/) { get; } | Mendapatkan GUID yang mengidentifikasi nilai ini di antara nilai lain dalam seluruh proyek. |
| [ValueId](../../aspose.tasks/outlinevalue/valueid/) { get; set; } | Mendapatkan atau mengatur Id unik dari nilai kode outline dalam sebuah proyek. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


