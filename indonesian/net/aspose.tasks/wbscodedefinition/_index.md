---
title: "Kelas WBSCodeDefinition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WBSCodeDefinition. Mewakili Definisi Kode WBS"
type: docs
weight: 3490
url: /id/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Mewakili Definisi Kode WBS.

```csharp
public class WBSCodeDefinition
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Menginisialisasi instance baru dari kelas `WBSCodeDefinition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Mendapatkan koleksi objek WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Mendapatkan atau mengatur awalan kode proyek. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menghasilkan kode WBS untuk tugas baru. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan memverifikasi keunikan kode WBS baru. |

## Contoh

Menampilkan cara menambahkan masker kode WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


