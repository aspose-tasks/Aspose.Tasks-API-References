---
title: "Enum WBSSequence"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.WBSSequence. Menentukan urutan untuk WBSCodeMask"
type: docs
weight: 3520
url: /id/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Menentukan urutan untuk WBSCodeMask

```csharp
public enum WBSSequence
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| OrderedNumbers | `0` | Menunjukkan urutan WBS angka. |
| OrderedUppercaseLetters | `1` | Menunjukkan urutan WBS huruf kapital. |
| OrderedLowercaseLetters | `2` | Menunjukkan urutan WBS huruf kecil. |
| UnorderedCharacters | `3` | Menunjukkan urutan WBS karakter tidak berurutan. |

## Contoh

Menampilkan cara mengatur urutan WBS.

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


