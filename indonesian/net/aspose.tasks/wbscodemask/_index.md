---
title: "Kelas WBSCodeMask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WBSCodeMask. Mewakili masker Kode WBS"
type: docs
weight: 3500
url: /id/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Mewakili masker Kode WBS.

```csharp
public class WBSCodeMask
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Menginisialisasi sebuah instance baru dari kelas `WBSCodeMask`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Mendapatkan atau mengatur jumlah karakter dari string kode. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Mendapatkan tingkat masker. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Mendapatkan atau mengatur pemisah string kode. Nilai default adalah titik. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Mendapatkan atau mengatur tipe karakter string kode. |

## Contoh

Menampilkan cara membuat masker kode WBS.

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

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


